cdist-type__consul_watch_nodes(7)
=================================

NAME
----
cdist-type__consul_watch_nodes - Manages consul nodes watches


DESCRIPTION
-----------
Generate and deploy watch definitions of type 'nodes' for a consul agent.
See http://www.consul.io/docs/agent/watches.html for parameter documentation.


REQUIRED PARAMETERS
-------------------
handler
   the handler to invoke when the data view updates


OPTIONAL PARAMETERS
-------------------
datacenter
   can be provided to override the agent's default datacenter

state
   if this watch is 'present' or 'absent'. Defaults to 'present'.

token
   can be provided to override the agent's default ACL token


EXAMPLES
--------

.. code-block:: sh

    __consul_watch_nodes some-id \
       --handler /usr/bin/my-key-handler.sh


SEE ALSO
--------
:manpage:`cdist-type__consul_agent`\ (7)

consul documentation at: <http://www.consul.io/docs/agent/watches.html>.


AUTHORS
-------
Steven Armstrong <steven-cdist--@--armstrong.cc>


COPYING
-------
Copyright \(C) 2015 Steven Armstrong. Free use of this software is
granted under the terms of the GNU General Public License version 3 (GPLv3).
