De:Portforwarding
=================

Date: 2013-03-11 23:51:48

/etc/rc.local is just the only method which works

← Nächstältere Version

Version vom 11. März 2013, 22:51 Uhr

Zeile 10:

Zeile 10:

 

 

 

<div>

Zu beachten ist, dass die Umleitung nur temporär ist und nach einem
Neustart des Rechners neu angelegt werden muss.

</div>

 

<div>

Zu beachten ist, dass die Umleitung nur temporär ist und nach einem
Neustart des Rechners neu angelegt werden muss.

</div>

−

<div>

 

</div>

\+

<div>

[Damit diese Umleitung automatisch nach jedem Neustart wirksam
wird]{.underline}, [muss]{.underline} die Zeile in /etc/rc.local [(vor
dem]{.underline} \'[exit 0]{.underline}\'[) eingetragen
werden]{.underline}.

</div>

−

<div>

~~Mit ein wenig mehr Aufwand ist es allerdings auch möglich~~, ~~die
Einstellung permanent zu machen:~~

</div>

\+

<div>

</div>

−

<div>

~~\*\[http://www.debian-administration.org/articles/445 Beschreibung für
auf Debian basierende Systeme\]~~

</div>

\+

<div>

</div>

−

<div>

 

</div>

\+

<div>

</div>

−

<div>

~~Man kann~~ die Zeile ~~auch \'\'\'~~in ~~die~~ /etc/rc.local
~~kopieren, damit sie bei jedem Systemstart ausgeführt wird\'~~\'\'.

</div>

\+

<div>

</div>

−

<div>

 

</div>

\+

<div>

</div>

 

 

 

<div>

\[\[Kategorie:De:Anleitung\]\]

</div>

 

<div>

\[\[Kategorie:De:Anleitung\]\]

</div>
