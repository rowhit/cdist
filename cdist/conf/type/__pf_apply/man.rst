cdist-type__pf_apply(7)
=======================

NAME
----
cdist-type__pf_apply - Apply pf(4) ruleset on \*BSD


DESCRIPTION
-----------
This type is used on \*BSD systems to manage the pf firewall's active ruleset.


REQUIRED PARAMETERS
-------------------
NONE


OPTIONAL PARAMETERS
-------------------
NONE


EXAMPLES
--------

.. code-block:: sh

    # Modify the ruleset on $__target_host:
    __pf_ruleset --state present --source /my/pf/ruleset.conf
    require="__pf_ruleset" \
       __pf_apply

    # Remove the ruleset on $__target_host (implies disabling pf(4):
    __pf_ruleset --state absent
    require="__pf_ruleset" \
       __pf_apply


SEE ALSO
--------
:manpage:`pf`\ (4), :manpage:`cdist-type__pf_ruleset`\ (7)


AUTHORS
-------
Jake Guffey <jake.guffey--@--eprotex.com>


COPYING
-------
Copyright \(C) 2012 Jake Guffey. Free use of this software is
granted under the terms of the GNU General Public License version 3 (GPLv3).
