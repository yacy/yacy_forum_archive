En:Portforwarding
=================

Date: 2014-06-04 13:53:15

Die Seite wurde neu angelegt: „You can configure any port for YaCy but
small numbers below 1024 are reserved to be used by \'\'\'root\'\'\' on
linux. Because some firewalls block port 8090 it can ..."

**Neue Seite**

<div>

You can configure any port for YaCy but small numbers below 1024 are
reserved to be used by \'\'\'root\'\'\' on linux.\
Because some firewalls block port 8090 it can be useful to redirect the
server port 80 to 8090.\
\
One solution for this is the usage of a port forwarding using iptables.
As user \'\'\'root\'\'\' just do\
\
iptables -t nat -A PREROUTING -p tcp \--dport 80 -j REDIRECT \--to-port
8090\
\
This is a temporary port redirection, if you want this to be permanent
just write this line into /etc/rc.local

</div>
