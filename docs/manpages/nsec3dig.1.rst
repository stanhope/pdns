nsec3dig
========

:program:`nsec3dig` - Show and validate NSEC3 proofs

Synopsis
--------

:program:`nsec3dig` *IPADDRESS* *PORT* *QNAME* *QTYPE* [recurse]

Description
-----------

:program:`nsec3dig` sends a query for *QNAME* and *QTYPE* to the nameserver at
*IPADDRESS* on port *PORT* and prints whether and why the NSEC3 proofs
are correct. Using the 'recurse' option sets the Recursion Desired (RD)
bit in the query.

Example
-------

``nsec3dig 8.8.8.8 53 doesntexist.isoc.nl TXT recurse``
