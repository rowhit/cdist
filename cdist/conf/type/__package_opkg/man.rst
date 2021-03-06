cdist-type__package_opkg(7)
===========================

NAME
----
cdist-type__package_opkg - Manage packages with opkg


DESCRIPTION
-----------
opkg is usually used on OpenWRT to manage packages.


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

    # Ensure lsof is installed
    __package_opkg lsof --state present

    # Remove obsolete package
    __package_opkg dnsmasq --state absent


SEE ALSO
--------
:manpage:`cdist-type__package`\ (7)


AUTHORS
-------
Giel van Schijndel <giel+cdist--@--mortis.eu>


COPYING
-------
Copyright \(C) 2012 Giel van Schijndel. Free use of this software is
granted under the terms of the GNU General Public License version 3 (GPLv3).
