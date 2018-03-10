Enabled displaying results after 14th page for local search queries.
====================================================================

Date: 2016-12-20 14:52:33

``` {style="white-space:pre-wrap;width:81ex"}
Enabled displaying results after 14th page for local search queries.

Fixes issue #90 for local queries only: Stealth mode, Portal mode or
Intranet mode. 
For P2p mode, the issue would probably be difficult to solve with
reasonable performance. This is still to dig.

Also switched some InterreputedException catch log messages to warn
level as this is normal behavior when shutting down a peer.

Fixed yacysearch buttons navbar behavior to deal correctly with total
results count or offset over 1000. Also improved the buttons navbar to
be able to navigate over 10th page for local queries.
```
