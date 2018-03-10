Firewall einrichten
===================

Date: 2013-09-22 00:03:28

[Yacy und der Router: ]{.autocomment} Ergänzung der Beschreibung zur
Einrichtung auf einem Speedport der Firma Telekom (Standardgerät)

← Nächstältere Version

Version vom 21. September 2013, 22:03 Uhr

Zeile 136:

Zeile 136:

 

 

 

<div>

{{Note\|Dieser Router unterstützt Universal Plug and Play (UPnP). Um die
Konfiguration zu vereinfachen, können Sie auch die integrierte
\[\[Firewall\_einrichten\#UPnP\_f.C3.A4higer\_Router\|UPnP
Unterstützung\]\] von YaCy aktivieren. }}

</div>

 

<div>

{{Note\|Dieser Router unterstützt Universal Plug and Play (UPnP). Um die
Konfiguration zu vereinfachen, können Sie auch die integrierte
\[\[Firewall\_einrichten\#UPnP\_f.C3.A4higer\_Router\|UPnP
Unterstützung\]\] von YaCy aktivieren. }}

</div>

−

<div>

</div>

 

−

<div>

</div>

 

−

<div>

~~=== SMC 7004ABR EU V2 ===~~

</div>

 

−

<div>

~~\[\[Bild:Smc7004.png\|thumb\]\]~~

</div>

 

−

<div>

~~Diese Beschreibung bezieht sich auf den Router 7004ABR EU V2 von
\[http://www.smc.com/ \]SMC mit der Firmware v1.018. Andere
Firmwareversionen weichen möglicherweise von dieser Beschreibung ab.~~

</div>

 

−

<div>

</div>

 

−

<div>

~~Der Router wird folgendermaßen konfiguriert:~~

</div>

 

−

<div>

</div>

 

−

<div>

~~\*Zunächst muss \'\'\'Advanced Setup\'\'\' gewählt werden.~~

</div>

 

−

<div>

~~\*Nun unter dem Punkt \'\'\'NAT\'\'\' den Unterpunkt \'\'\'Virtual
Server\'\'\' auswählen.~~

</div>

 

−

<div>

~~\*Jetzt muss der Wert für die \'\'\'IP-Adresse\'\'\' (die Adresse des
Rechners, auf dem YaCy läuft) eingegeben werden. \'\'\'Protocol
Type\'\'\' bleibt auf TCP eingestellt. Nun unter \'\'\'LAN Port\'\'\'
den Port einstellen, an dem YaCy auf dem Rechner, auf dem es läuft,
erreichbar ist (normalerweise 8090) und unter \'\'\'Public Port\'\'\'
den Port angeben, von dem aus YaCy aus dem Internet erreichbar sein soll
(normalerweise 8090). Im Feld \'\'\'Enable\'\'\' muss der Haken gesetzt
sein. (Siehe Screenshot!)~~

</div>

 

−

<div>

~~\*Nun noch mit einen Druck auf \'\'\'Add\'\'\' bestätigen.~~

</div>

 

−

<div>

</div>

 

−

<div>

~~Jetzt sollten die Angaben nochmals überprüft und gegebenenfalls
korrigiert oder gelöscht werden.~~

</div>

 

 

 

 

 

Zeile 189:

Zeile 175:

 

<div>

Weiterführende Informationen sind auf der folgenden Seite zu finden.
\[http://www.netgear.de/Support/Anleitungen/ NETGEAR Anleitungen
Deutsch\]

</div>

 

<div>

Weiterführende Informationen sind auf der folgenden Seite zu finden.
\[http://www.netgear.de/Support/Anleitungen/ NETGEAR Anleitungen
Deutsch\]

</div>

 

 

 

\+

<div>

[=== SMC 7004ABR EU V2 ===]{.underline}

</div>

 

\+

<div>

[\[\[Bild:Smc7004.png\|thumb\]\]]{.underline}

</div>

 

\+

<div>

[Diese Beschreibung bezieht sich auf den Router 7004ABR EU V2 von
\[http://www.smc.com/ \]SMC mit der Firmware v1.018. Andere
Firmwareversionen weichen möglicherweise von dieser Beschreibung
ab.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Der Router wird folgendermaßen konfiguriert:]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[\*Zunächst muss \'\'\'Advanced Setup\'\'\' gewählt werden.]{.underline}

</div>

 

\+

<div>

[\*Nun unter dem Punkt \'\'\'NAT\'\'\' den Unterpunkt \'\'\'Virtual
Server\'\'\' auswählen.]{.underline}

</div>

 

\+

<div>

[\*Jetzt muss der Wert für die \'\'\'IP-Adresse\'\'\' (die Adresse des
Rechners, auf dem YaCy läuft) eingegeben werden. \'\'\'Protocol
Type\'\'\' bleibt auf TCP eingestellt. Nun unter \'\'\'LAN Port\'\'\'
den Port einstellen, an dem YaCy auf dem Rechner, auf dem es läuft,
erreichbar ist (normalerweise 8090) und unter \'\'\'Public Port\'\'\'
den Port angeben, von dem aus YaCy aus dem Internet erreichbar sein soll
(normalerweise 8090). Im Feld \'\'\'Enable\'\'\' muss der Haken gesetzt
sein. (Siehe Screenshot!)]{.underline}

</div>

 

\+

<div>

[\*Nun noch mit einen Druck auf \'\'\'Add\'\'\' bestätigen.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Jetzt sollten die Angaben nochmals überprüft und gegebenenfalls
korrigiert oder gelöscht werden.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[=== Speedport W 723V (und ggf. andere Speedport-Geräte der Telekom)
===]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Standardgemäß ist der Port 8090 nicht offen und damit nur die Teilnahme
als Julior an YaCy möglich.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Die Einrichtung einer Portweiterleitung ist wie folgt
möglich.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[\# Router-Konfigurationsmenü über den Browser öffnen, Adresse eingeben:
speedport.ip]{.underline}

</div>

 

\+

<div>

[\# Im linken Menü auf den Punkt \'\'\'Netzwerk\'\'\']{.underline}

</div>

 

\+

<div>

[\# Hier auf den Punkt \'\'\'NAT & Portregeln\'\'\']{.underline}

</div>

 

\+

<div>

[\# Auf \'\'\'Weitere Portregel hinzufügen\'\'\' klicken]{.underline}

</div>

 

\+

<div>

[\# beliebige Bezeichnung eingeben, z.B. \"Portregel YaCy\"]{.underline}

</div>

 

\+

<div>

[\# Art der Regel einstellen: \"Port Weiterleitung\"]{.underline}

</div>

 

\+

<div>

[\# Bei \"Gültig für Gerät\" den Namen des eigenen PC
eingeben]{.underline}

</div>

 

\+

<div>

[\# bei TCP-Portbereich und UDP-Portbereich die Portnummer 8090
eingeben]{.underline}

</div>

 

\+

<div>

[\# Auf speichern klicken, ca. 60 Sekunden warten, ggf. Router
neustarten]{.underline}

</div>

 

\+

<div>

[\# in YaCy testen, ob es funktioniert hat]{.underline}

</div>

 

 

 

<div>

\[\[Kategorie:De:Einrichtung\]\]

</div>

 

<div>

\[\[Kategorie:De:Einrichtung\]\]

</div>

 

<div>

\[\[Kategorie:De:Anleitung\]\]

</div>

 

<div>

\[\[Kategorie:De:Anleitung\]\]

</div>
