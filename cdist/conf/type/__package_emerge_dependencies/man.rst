cdist-type__package_emerge_dependencies(7)
==========================================

NAME
----
cdist-type__package_emerge_dependencies - Install dependencies for __package_emerge


DESCRIPTION
-----------
Portage is usually used on the gentoo distribution to manage packages.
This type installs the following tools which are required by __package_emerge to work:

* app-portage/flaggie
* app-portage/gentoolkit


REQUIRED PARAMETERS
-------------------
None


OPTIONAL PARAMETERS
-------------------
None


EXAMPLES
--------

.. code-block:: sh

    # Ensure app-portage/flaggie and app-portage/gentoolkit are installed
    __package_emerge_dependencies


SEE ALSO
--------
:manpage:`cdist-type__package`\ (7), :manpage:`cdist-type__package_emerge`\ (7)


AUTHORS
-------
Thomas Oettli <otho--@--sfs.biz>


COPYING
-------
Copyright \(C) 2013 Thomas Oettli. Free use of this software is
granted under the terms of the GNU General Public License version 3 (GPLv3).
