Firewall einrichten
===================

Date: 2015-05-31 17:41:27

Anleitung für EasyBox 804 hinzugefügt

← Nächstältere Version

Version vom 31. Mai 2015, 15:41 Uhr

Zeile 82:

Zeile 82:

 

 

 

<div>

Nun erscheint die Übersichtsseite, auf der kontrolliert werden kann, ob
alle Angaben richtig sind und wo die Weiterleitung gegebenenfalls
geändert oder wieder gelöscht werden kann.

</div>

 

<div>

Nun erscheint die Übersichtsseite, auf der kontrolliert werden kann, ob
alle Angaben richtig sind und wo die Weiterleitung gegebenenfalls
geändert oder wieder gelöscht werden kann.

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[=== easy.box 804 ===]{.underline}

</div>

 

\+

<div>

[\[\[Datei:EasyBox\_804.png\|thumb\|Port-Mapping in easy.box
804\]\]]{.underline}

</div>

 

\+

<div>

[Um eine Portfreigabe in der easy.box zu konfigurieren, empfiehlt es
sich, dem betreffenden Rechner zunächst über statisches DHCP eine feste
lokale IP-Adresse zuzuordnen:]{.underline}

</div>

 

\+

<div>

[\* Wählen Sie im Menü den Eintrag \"Übersicht\".]{.underline}

</div>

 

\+

<div>

[\* Klicken Sie auf das Symbol \"Heimnetzwerk\".]{.underline}

</div>

 

\+

<div>

[\* Scrollen Sie nach unten zum Punkt \"Statisches DHCP -
Heimnetzwerk\".]{.underline}

</div>

 

\+

<div>

[\* Klicken Sie auf das Plus-Symbol.]{.underline}

</div>

 

\+

<div>

[\* Hier sollte im Pull-Down-Menü das gewünschte Gerät angezeigt werden.
Falls nicht prüfen Sie, ob das Gerät eingeschaltet und verbunden ist.
Evtl. hilft ein Neustart der easy.box (=\> Status & Hilfe =\> Neustart).
Die Mac-Adresse wird dann automatisch eingetragen. Tragen Sie eine
geeignete lokale IP-Adresse ein.]{.underline}

</div>

 

\+

<div>

[\* Scrollen Sie ganz nach unten und klicken Sie auf
\"Bestätigen\".]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Nun kann die Portfreigabe konfiguriert werden:]{.underline}

</div>

 

\+

<div>

[\* Wählen Sie im Menü den Eintrag \"Internet\".]{.underline}

</div>

 

\+

<div>

[\* Wählen Sie in der Navigationsleiste den Eintrag
\"Port-Mapping\".]{.underline}

</div>

 

\+

<div>

[\* Klicken Sie auf das Plus-Symbol.]{.underline}

</div>

 

\+

<div>

[\* Unter \"Gerät\" sollte im Pull-Down-Menü wieder der entsprechende
Rechner angezeigt werden (sonst vorgehen wie oben).]{.underline}

</div>

 

\+

<div>

[\* Wenn das Gerät ausgewählt wurde, wird die lokale IP-Adresse
automatisch eingefügt.]{.underline}

</div>

 

\+

<div>

[\* Wählen Sie als Protokoll \"UPD\".]{.underline}

</div>

 

\+

<div>

[\* Tragen Sie unter \"Öffentlicher Port\" und unter \"Lokaler Port\"
jeweils \"8090\" (bzw. \"8443\" für https) ein.]{.underline}

</div>

 

\+

<div>

[\* Klicken Sie auf die Schaltfläche \"Speichern\".]{.underline}

</div>

 

\+

<div>

[\* Klicken Sie auf der Seite \"Port-Mapping\" auf die Schaltfläche
\"Bestätigen\".]{.underline}

</div>

 

\+

<div>

[\* Wichtig: Starten Sie die easy.box neu (=\> Status & Hilfe =\>
Neustart).]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Hinweis: Wenn man zum Testen der Portfreigabe in der URL-Leiste des
Browsers die öffentliche IP-Adresse und den Port eingibt, erhält man
eine Fehlermeldung \"Unable to connect\", wenn der damit verbundene
HTTP-Request über das gleiche Gateway geroutet wird, in der auch das
Port-Mapping konfiguriert wurde
\[https://forum.vodafone.de/t5/Festnetz-Ger%C3%A4te-z-B-EasyBox/EasyBox-804-DDNS-Port-Mapping-funktioniert-nicht/td-p/816308\].
Beim Testen von einem fremden Internetzugang, sollte der Zugang zur
Weboberfläche des YaCy-Peers klappen.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Damit in der YaCy-Adminkonsole die neue Konfiguration des Ports auch
angezeigt wird, ist evtl. ein Neustart des YaCy-Peers
nötig.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

 

 

<div>

=== Eumex 300 IP ===

</div>

 

<div>

=== Eumex 300 IP ===

</div>
