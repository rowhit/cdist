cdist-type__package_emerge(7)
=============================

NAME
----
cdist-type__package_emerge - Manage packages with portage


DESCRIPTION
-----------
Portage is usually used on the gentoo distribution to manage packages.
This type requires app-portage/gentoolkit installed on the target host.
cdist-type__package_emerge_dependencies is supposed to install the needed
packages on the target host.


REQUIRED PARAMETERS
-------------------
None


OPTIONAL PARAMETERS
-------------------
name
    If supplied, use the name and not the object id as the package name.

state
    Either "present" or "absent", defaults to "present".

version
    If supplied, use to install or uninstall a specific version of the package named.

EXAMPLES
--------

.. code-block:: sh

    # Ensure sys-devel/gcc is installed
    __package_emerge sys-devel/gcc --state present

    # If you want a specific version of a package
    __package_emerge app-portage/gentoolkit --state present --version 0.3.0.8-r2

    # Remove package
    __package_emerge sys-devel/gcc --state absent


SEE ALSO
--------
:manpage:`cdist-type__package`\ (7), :manpage:`cdist-type__package_emerge_dependencies`\ (7)


AUTHORS
-------
Thomas Oettli <otho--@--sfs.biz>


COPYING
-------
Copyright \(C) 2013 Thomas Oettli. Free use of this software is
granted under the terms of the GNU General Public License version 3 (GPLv3).
