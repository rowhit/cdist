cdist-type__cdist(7)
====================

NAME
----
cdist-type__cdist - Manage cdist installations


DESCRIPTION
-----------
This cdist type allows you to easily setup cdist
on another box, to allow the other box to configure
systems.

This type is *NOT* required by target hosts.
It is only helpful to build FROM which you configure
other hosts.

This type will use git to clone


REQUIRED PARAMETERS
-------------------

OPTIONAL PARAMETERS
-------------------
username
    Select the user to create for the cdist installation.
    Defaults to "cdist".

source
    Select the source from which to clone cdist from.
    Defaults to "git://github.com/telmich/cdist.git".


branch
    Select the branch to checkout from.
    Defaults to "master".


EXAMPLES
--------

.. code-block:: sh

    # Install cdist for user cdist in her home as subfolder cdist
    __cdist /home/cdist/cdist

    # Use alternative source
    __cdist --source "git://git.schottelius.org/cdist" /home/cdist/cdist


AUTHORS
-------
Nico Schottelius <nico-cdist--@--schottelius.org>


COPYING
-------
Copyright \(C) 2013 Nico Schottelius. Free use of this software is
granted under the terms of the GNU General Public License version 3 (GPLv3).
