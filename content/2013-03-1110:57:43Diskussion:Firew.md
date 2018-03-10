Diskussion:Firewall einrichten
==============================

Date: 2013-03-11 10:57:43

port fix

← Nächstältere Version

Version vom 11. März 2013, 09:57 Uhr

Zeile 19:

Zeile 19:

 

<div>

=== Arno\'s IPtables Firewall Script ===

</div>

 

<div>

=== Arno\'s IPtables Firewall Script ===

</div>

 

<div>

Hier muss die Datei /etc/arno-iptables-firewall/firewall.conf nur
abgeaendert und dann das init-Script mit restart aufgerufen werden. In
der besagten Datei wird als erstes die Option NAT\_FORWARD\_TCP (YaCy
kommt derzeit ohne UDP, also braucht NAT\_FORWARD\_UDP nicht angefasst
zu werden) erweitert:

</div>

 

<div>

Hier muss die Datei /etc/arno-iptables-firewall/firewall.conf nur
abgeaendert und dann das init-Script mit restart aufgerufen werden. In
der besagten Datei wird als erstes die Option NAT\_FORWARD\_TCP (YaCy
kommt derzeit ohne UDP, also braucht NAT\_FORWARD\_UDP nicht angefasst
zu werden) erweitert:

</div>

−

<div>

\<pre\>\<nowiki\>NAT\_FORWARD\_TCP=\"~~8080~~\>a.b.c.\"\</nowiki\>\</pre\>

</div>

\+

<div>

\<pre\>\<nowiki\>NAT\_FORWARD\_TCP=\"[8090]{.underline}\>a.b.c.\"\</nowiki\>\</pre\>

</div>

−

<div>

Wobei a.b.c.d wieder die private IP eurer YaCy-Node ist und ~~8080~~ der
Port, unter dem YaCy erreichbar ist (sollte eurer ISP den Zugriff auf
diesen Port zu drosseln oder gar zu unterbinden, sucht euch einfach
einen anderen aus! :-) ). Auch hier brauchte der gesamte PC nicht
neugestartet werden:

</div>

\+

<div>

Wobei a.b.c.d wieder die private IP eurer YaCy-Node ist und
[8090]{.underline} der Port, unter dem YaCy erreichbar ist (sollte eurer
ISP den Zugriff auf diesen Port zu drosseln oder gar zu unterbinden,
sucht euch einfach einen anderen aus! :-) ). Auch hier brauchte der
gesamte PC nicht neugestartet werden:

</div>

 

<div>

\<pre\>\<nowiki\>/etc/init.d/arno-iptables-firewall
restart\</nowiki\>\</pre\>

</div>

 

<div>

\<pre\>\<nowiki\>/etc/init.d/arno-iptables-firewall
restart\</nowiki\>\</pre\>

</div>

 

 
