Dev:APIHttpHeader
=================

Date: 2013-11-29 01:36:38

yacyh domain names

**Neue Seite**

<div>

== HTTP Header Attributes for YaCy API calls ==\
When calling a remote peer the standard HTTP/1.1 header properties are
sufficient.\
\
=== The Host-Attribute ===\
There is the HTTP/1.1-required \'Host\'-Attribute which can be filled
with the IP of the called peer.\
The caller should put the peer\'s virtual HexHash domain name of the
called peer in this \'Host\' attribute, if the called peer can operate
as \[\[Dev:PeerType\#mentor\|mentor peer\]\] and the caller wants to
address this feature.\
The \[\[Dev:EnhancedBase64\|Enhanced Base64-encoded\]\] peer hash is
encoded as \[\[Dev:HexHash\|HexHash\]\] and the host name is created
using this HexHash with an appended \'.yacyh\' extension. A Host
property in the http header looks like\
Host: d7841c7477a57de875.yacyh\
This is only necessary if the called host is a
\[\[Dev:PeerType\#mentor\|mentor peer\]\] and the target host is a
\[\[Dev:PeerType\#mentee\|mentee peer\]\].

</div>
