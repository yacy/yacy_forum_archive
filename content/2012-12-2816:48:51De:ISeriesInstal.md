De:ISeriesInstall
=================

Date: 2012-12-28 16:48:51

Release von V5R2M0 auf V5R3M0 geändert, da es unter V5R2 kein Java 1.5
gibt.

← Nächstältere Version

Version vom 28. Dezember 2012, 15:48 Uhr

Zeile 2:

Zeile 2:

 

<div>

== Konfiguration Java 1.5 ==

</div>

 

<div>

== Konfiguration Java 1.5 ==

</div>

 

<div>

Zur Installation wird mindestens die Java Version 1.5 benötigt. Es
handelt sich hierbei um das kostenfreie IBM Lizenzprogramm 5722JV1
Option 7.

</div>

 

<div>

Zur Installation wird mindestens die Java Version 1.5 benötigt. Es
handelt sich hierbei um das kostenfreie IBM Lizenzprogramm 5722JV1
Option 7.

</div>

−

<div>

Zur Aktivierung der installierten Java Version 1.5 auf einer AS/400
Maschine mit ~~V5R2M0~~ muss die Datei SystemDefault.properties im
Verzeichnis /qibm/UserData/Java400 erstellt werden. Folgender Inhalt
muss der Datei hinzugefügt werden: \<br /\>

</div>

\+

<div>

Zur Aktivierung der installierten Java Version 1.5 auf einer AS/400
Maschine mit [V5R3M0]{.underline} muss die Datei
SystemDefault.properties im Verzeichnis /qibm/UserData/Java400 erstellt
werden. Folgender Inhalt muss der Datei hinzugefügt werden: \<br /\>

</div>

 

<div>

\'\'\'java.version=1.5\'\'\' \<br /\>

</div>

 

<div>

\'\'\'java.version=1.5\'\'\' \<br /\>

</div>

 

<div>

Zur Überprüfung der Java Version kann anschließend folgender Command in
der QSH ausgeführt werden: \<br /\>

</div>

 

<div>

Zur Überprüfung der Java Version kann anschließend folgender Command in
der QSH ausgeführt werden: \<br /\>

</div>
