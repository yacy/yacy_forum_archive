Started implementing optional https preference for protocol operations
======================================================================

Date: 2017-12-15 11:28:46

``` {style="white-space:pre-wrap;width:81ex"}
Started implementing optional https preference for protocol operations

Introduced through the new configurable setting
network.unit.protocol.https.preferred, defaulting to false for now.

Let choose to prefer using https when available on remote peers to
perform YaCy protocol operations including notably hello or transferRWI.

Not yet implemented for every YaCy protocol operations.
```
