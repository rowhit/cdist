cdist-type__package_pacman(7)
=============================

NAME
----
cdist-type__package_pacman - Manage packages with pacman


DESCRIPTION
-----------
Pacman is usually used on the Archlinux distribution to manage packages.


REQUIRED PARAMETERS
-------------------
None


OPTIONAL PARAMETERS
-------------------
name
    If supplied, use the name and not the object id as the package name.

state
    Either "present" or "absent", defaults to "present"


EXAMPLES
--------

.. code-block:: sh

    # Ensure zsh in installed
    __package_pacman zsh --state present

    # If you don't want to follow pythonX packages, but always use python
    __package_pacman python --state present --name python2

    # Remove obsolete package
    __package_pacman puppet --state absent


SEE ALSO
--------
:manpage:`cdist-type__package`\ (7)


AUTHORS
-------
Nico Schottelius <nico-cdist--@--schottelius.org>


COPYING
-------
Copyright \(C) 2011-2012 Nico Schottelius. Free use of this software is
granted under the terms of the GNU General Public License version 3 (GPLv3).
