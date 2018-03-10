Diskussion:Firewall einrichten
==============================

Date: 2013-11-27 12:11:45

port 8090 fix

← Nächstältere Version

Version vom 27. November 2013, 11:11 Uhr

Zeile 13:

Zeile 13:

 

<div>

chmod u+x 04-yacy.sh

</div>

 

<div>

chmod u+x 04-yacy.sh

</div>

 

<div>

(eventuell noch umbenennen!)\</nowiki\>\</pre\>

</div>

 

<div>

(eventuell noch umbenennen!)\</nowiki\>\</pre\>

</div>

−

<div>

Dann geht es mit dem Editieren des gerade runtergeladenen Scriptes
weiter, denn ihr muesst a.b.c.d und ~~8080~~ gegen eure private IP eures
Rechners austauschen (eventuell auch Port). Anschliessend wird Bastille
neugestartet:

</div>

\+

<div>

Dann geht es mit dem Editieren des gerade runtergeladenen Scriptes
weiter, denn ihr muesst a.b.c.d und [8090]{.underline} gegen eure
private IP eures Rechners austauschen (eventuell auch Port).
Anschliessend wird Bastille neugestartet:

</div>

 

<div>

\<pre\>\<nowiki\>/etc/init.d/bastille-firewall start\</nowiki\>\</pre\>

</div>

 

<div>

\<pre\>\<nowiki\>/etc/init.d/bastille-firewall start\</nowiki\>\</pre\>

</div>

 

<div>

\"restart\" scheint wohl broken zu sein, \"start\" sollte hier aber auch
zum gleichen Ergebnis fuehren. Das sollte es schon gewesen sein.

</div>

 

<div>

\"restart\" scheint wohl broken zu sein, \"start\" sollte hier aber auch
zum gleichen Ergebnis fuehren. Das sollte es schon gewesen sein.

</div>
