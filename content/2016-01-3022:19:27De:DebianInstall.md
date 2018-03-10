De:DebianInstall
================

Date: 2016-01-30 22:19:27

← Nächstältere Version

Version vom 30. Januar 2016, 21:19 Uhr

(Eine dazwischenliegende Version von einem Benutzer wird nicht
angezeigt)

Zeile 19:

Zeile 19:

 

<div>

  apt-get install openjdk-7-jre-headless \# die headless Java Version
reicht aus

</div>

 

<div>

  apt-get install openjdk-7-jre-headless \# die headless Java Version
reicht aus

</div>

 

<div>

  apt-get install yacy

</div>

 

<div>

  apt-get install yacy

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Bei der Installatin werden folgende Informationen abgefragt, die
nachträglich im \[\[\#YaCy-Webinterface aufrufen\|YaCy-Webinterface\]\]
in der Administratorbereich unter First Steps geändert werden
können:]{.underline}

</div>

 

\+

<div>

[\* Name für den YaCy-Peer]{.underline}

</div>

 

\+

<div>

[\* Admin-Passwort]{.underline}

</div>

 

\+

<div>

[\* Wahl des Netzwerks (freeworld\|
intranet\|allip\|webportal\|url)]{.underline}

</div>

 

\+

<div>

[\* Initial Memory for java virtual mashine (180 MB
empfohlen)]{.underline}

</div>

 

\+

<div>

[\* Maximum memory for java virtual mashine (600 MB
empfohlen)]{.underline}

</div>

 

<div>

YaCy wird bei der Installation als Dienst in /etc/init.d eingetragen, so
dass YaCy bei einem Debian-Startup automatisch gestartet, und bei einem
Shutdown auch beendet wird.\<br /\>

</div>

 

<div>

YaCy wird bei der Installation als Dienst in /etc/init.d eingetragen, so
dass YaCy bei einem Debian-Startup automatisch gestartet, und bei einem
Shutdown auch beendet wird.\<br /\>

</div>

 

<div>

Man kann YaCy auch manuell starten, stoppen und neustarten:

</div>

 

<div>

Man kann YaCy auch manuell starten, stoppen und neustarten:

</div>

Zeile 26:

Zeile 33:

 

<div>

\<br /\>

</div>

 

<div>

\<br /\>

</div>

 

 

−

<div>

 

</div>

\+

<div>

==YaCy-[Webinterface]{.underline} aufrufen==

</div>

−

<div>

==YaCy-~~Web-Interface~~ aufrufen==

</div>

\+

<div>

</div>

 

<div>

YaCy läuft per default auf Port 8090, die Adresse für die Administration
ist dann

</div>

 

<div>

YaCy läuft per default auf Port 8090, die Adresse für die Administration
ist dann

</div>

 

<div>

  http://localhost:8090/

</div>

 

<div>

  http://localhost:8090/

</div>

 

<div>

\<br /\>

</div>

 

<div>

\<br /\>

</div>

−

<div>

</div>

 

 

<div>

Das YaCy-HOME-Verzeichnis ist dann /usr/share/yacy

</div>

 

<div>

Das YaCy-HOME-Verzeichnis ist dann /usr/share/yacy

</div>

 

<div>

Das Datenverzeichnis DATA befindet sich im YaCy-Home-Verzeichnis.

</div>

 

<div>

Das Datenverzeichnis DATA befindet sich im YaCy-Home-Verzeichnis.

</div>

 

\+

<div>

[\<br /\>]{.underline}

</div>

 

<div>

\<br /\>

</div>

 

<div>

\<br /\>

</div>

 

 
