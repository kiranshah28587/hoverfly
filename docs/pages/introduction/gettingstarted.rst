.. _getting_started:

Getting Started
===============

.. sidebar:: Note

    It is recommended that you keep Hoverfly and hoverctl in the same directory. However if they are not in the same directory, hoverctl will look in the current directory for Hoverfly, then in other directories on the PATH.


Hoverfly is composed of two binaries: Hoverfly, and hoverctl.

hoverctl can be used to spawn, configure, control, and stop Hoverfly. It allows you to run Hoverfly as a daemon.

Hoverfly is the application that does the bulk of the work, providing the proxy server or webserver and the API endpoints.

Once you have extracted both Hoverfly and hoverctl into a directory on your PATH, you can run hoverctl and Hoverfly.

.. code:: bash

    hoverctl --version
    hoverfly --version

If installed correctly, both of these commands should return a version number. Now you can run an instance of Hoverfly:

.. code:: bash

    hoverctl start

Check whether Hoverfly is running with the following command:

.. code:: bash

    hoverctl logs

The logs should contain the string ``serving proxy`` which indicates that Hoverfly is up and running.

Finally, stop Hoverfly with:

.. code:: bash

    hoverctl stop
