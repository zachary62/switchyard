Switchyard
==========

Switchyard is a library and framework for creating networked systems in Python.  It is primarily intended for educational use and supports creating devices from layer 2 (Ethernet) all the way through the application layer.

Documentation is available at http://cs.colgate.edu/~jsommers/switchyard
Documentation is written using the Python Sphinx package; doc sources are
available in the documentation directory.

Switchyard can run in a standalone test harness mode, or can also use "live" network interfaces on a Linux or macos host.  It works nicely within Mininet and other virtual host environments.  The version of Switchyard on the master branch is a major revision of the code as of the end of 2016.  This is the second major overhaul.  The earliest working version of Switchyard (from late 2013) can be found on the v1 branch, and the subsequent rewrite (through the end of 2016) can be found on the v2 branch.  Many parts of the code are under active development.  As with the last major version of Switchyard, this one requires Python 3.4, at minimum.

Installation
------------

Prequisites: on Ubuntu and Fedora systems, you'll also likely need to install additional packages (do this before using pip to install the Python libraries).  The list of libraries below is for recent versions of Ubuntu (14.04 and later) and Fedora (20 and later):

 * Ubuntu: `sudo apt-get install libffi-dev libpcap-dev python3-dev`
 * Fedora: `sudo yum install libffi-devel libpcap-devel python3-devel`

You can either install Switchyard and the related necessary libraries in the system Python directories (ok, but often less desirable) or in a venv (Python virtual installation environment).  The venv route is highly suggested, since it makes all installation "local" and easily destroyed, cleaned up, and recreated.

To create a new virtual environment, you could do something like the following:

    $ python3 -m venv syenv

You can change the name "syenv" to whatever you'd like to name your virtual environment.  Next, you need to activate the environment.  The instructions vary depending on the shell you're using.  On bash, the command is:

    $ source ./syenv/bin/activate

You'll need to replace syenv with whatever you named the virtual environment.  If you're using a different shell than bash, refer to Python documentation on the venv module.

Finally, install Switchyard.  All the required additional libraries should be automatically installed, too.

    $ pip3 install switchyard


Documentation and Exercises
---------------------------
 
 * Documentation sources can be found in the documentation directory.  See
   http://cs.colgate.edu/~jsommers/switchyard for compiled/built docs.

 * Sample exercises (in ReStructuredText format) can be found in the
   examples/exercises directory.  

 * Instructor-only materials such as test scenarios and other scripts
   available on request to the author of Switchyard (jsommers@colgate.edu).

Credits
-------

I gratefully acknowledge support from the NSF.  The materials here are
based upon work supported by the National Science Foundation under
grant CNS-1054985 ("CAREER: Expanding the functionality of Internet
routers").

Any opinions, findings, and conclusions or recommendations expressed
in this material are those of the author and do not necessarily
reflect the views of the National Science Foundation.

License
-------

This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. 
http://creativecommons.org/licenses/by-nc-sa/4.0/
