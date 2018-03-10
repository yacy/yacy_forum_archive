De:WindowsInstall
=================

Date: 2015-11-19 15:06:44

← Nächstältere Version

Version vom 19. November 2015, 14:06 Uhr

(Eine dazwischenliegende Version von einem Benutzer wird nicht
angezeigt)

Zeile 4:

Zeile 4:

 

<div>

===YaCy-Installer===

</div>

 

<div>

===YaCy-Installer===

</div>

 

<div>

\[\[Bild:DownloadWindowsInstaller.png\|thumb\]\]

</div>

 

<div>

\[\[Bild:DownloadWindowsInstaller.png\|thumb\]\]

</div>

−

<div>

Der Windows-Installer steht auf der \[http://yacy.net YaCy-Seite\] zum
Download zur Verfügung (siehe Abbildung). Damit kann YaCy auf dem unter
Windows üblichen Weg mit einer .exe-Datei installiert werden.\<br /\>

</div>

\+

<div>

Der Windows-Installer steht auf der \[http://yacy.net YaCy-Seite\] zum
Download zur Verfügung (siehe Abbildung). Damit kann YaCy auf dem unter
Windows üblichen Weg mit einer .exe-Datei installiert werden.[\<br
/\>]{.underline}\<br /\>

</div>

−

<div>

Bei der Installation wird überprüft, ob die benötigte
Java-Laufzeitumgebung bereits installiert ist. Ist dies nicht der Fall,
wird diese automatisch nachgeladen und installiert. Sollten für die
Installation von YaCy keine Administrator-Rechte vorliegen, wird die
Java-Installation in den Ordner \"Gemeinsame Dokumente\" (XP) bzw.
\"Öffentliche Dokumente\" (Vista) abgelegt. Von dort kann dann ein
Administrator Java auf dem System installieren.\<br /\>

</div>

\+

<div>

Bei der Installation wird überprüft, ob die benötigte
Java-Laufzeitumgebung bereits installiert ist. Ist dies nicht der Fall,
wird diese automatisch nachgeladen und installiert. Sollten für die
Installation von YaCy keine Administrator-Rechte vorliegen, wird die
Java-Installation in den Ordner \"Gemeinsame Dokumente\" (XP) bzw.
\"Öffentliche Dokumente\" (Vista) abgelegt. Von dort kann dann ein
Administrator Java auf dem System installieren. [Um dies zu vermeiden,
kann die yacy\_\<version\>.exe mit Administratorrechten ausgeführt
werden.\<br /\>]{.underline}\<br /\>

</div>

−

<div>

YaCy wird standardmäßg in das Verzeichnis
C:\\users\\\<Benutzername\>\\YaCy installiert. ~~Auf~~ dem Deskop
~~werden~~ ein YaCy-Icon und im Startmenü ein YaCy-Eintrag angelegt.

</div>

\+

<div>

YaCy wird standardmäßg in das Verzeichnis
C:\\users\\\<Benutzername\>\\YaCy installiert. [Wenn bei der
Installation manuell ein Installationspfad ausgewählt wird, der nicht
innnerhalb von C:\\users\\\<Benutzername\> liegt, sind zum Starten von
YaCy ggf. Administratorrechte nötig, wovon abzuraten ist. Bei der
Installation werden auf]{.underline} dem Deskop ein YaCy-Icon und im
Startmenü ein YaCy-Eintrag angelegt[, mit denen man
\[\[De:FirstStart\|YaCy starten\]\] kann.\<br /\>\<br /\>]{.underline}

</div>

 

\+

<div>

[Um YaCy zu deinstallieren, muss ggf. zunächst
\[\[De:WindowsInstall\#YaCy als Windows Service\|YaCy als Windows
Service\]\] deinstalliert werden. Danach kann YaCy über das Startmenü
=\> Alle Programme =\> YaCy =\> Uninstall deinstalliert
werden]{.underline}.  

</div>

 

 

−

<div>

~~\<br /\>\<br /\>~~\<br /\>\<br /\>

</div>

\+

<div>

\<br /\>\<br /\>

</div>

 

 

 

<div>

===YaCy-Archiv===

</div>

 

<div>

===YaCy-Archiv===

</div>

 

<div>

\[\[Bild:DownloadGenericPackage.png\|thumb\]\]

</div>

 

<div>

\[\[Bild:DownloadGenericPackage.png\|thumb\]\]

</div>

−

<div>

YaCy kann auch mit dem generischen Paket, das für alle Betriebssysteme
geeignet ist, installiert werden. Es steht auf der \[http://yacy.net
YaCy-Seite\] zum Download zur Verfügung (siehe Abbildung). \<br /\>

</div>

\+

<div>

YaCy kann auch mit dem generischen Paket, das für alle Betriebssysteme
geeignet ist, installiert werden. Es steht auf der \[http://yacy.net
YaCy-Seite\] zum Download zur Verfügung (siehe Abbildung). [\<br
/\>]{.underline}\<br /\>

</div>

−

<div>

Zum Entpacken muss ein geeignetes Programm installiert sein (z.B.
\[http://www.7-zip.org 7zip\] FilZip, WinZip oder WinRAR). Das Archiv
(Dateiendung .tar.gz) kann in ein geeignetes Verzeichnis unterhalb von
C:\\users\\\<Benutzername\> kopiert werden, um es dann mit Rechtsklick
und \"hier entpacken\" zu entpacken. Ggf. wird es im ersten Schritt nur
dekomprimiert und man erhält eine Archiv-Datei (Dateiendung .tar). Diese
Archiv-Datei muss erneut entpackt werden, um das yacy-Verzeicnhis zu
extrahieren.\<br /\>

</div>

\+

<div>

Zum Entpacken muss ein geeignetes Programm installiert sein (z.B.
\[http://www.7-zip.org 7zip\][,]{.underline}FilZip, WinZip oder WinRAR).
Das Archiv (Dateiendung .tar.gz) kann in ein geeignetes Verzeichnis
unterhalb von C:\\users\\\<Benutzername\> kopiert werden, um es dann mit
Rechtsklick und \"hier entpacken\" zu entpacken. Ggf. wird es im ersten
Schritt nur dekomprimiert und man erhält eine Archiv-Datei (Dateiendung
.tar). Diese Archiv-Datei muss erneut entpackt werden, um das
yacy-Verzeicnhis zu extrahieren.\<br /\>

</div>

−

<div>

Beispiel: yacy\_v1.82.tar.gz (komprimiertes Archiv) =\> entpacken =\>
yacy\_v1.82.tar (Archiv-Datei)=\> entpacken =\> yacy (Verzeichnis)

</div>

\+

<div>

Beispiel: yacy\_v1.82.tar.gz (komprimiertes Archiv) =\> entpacken =\>
yacy\_v1.82.tar (Archiv-Datei)=\> entpacken =\> yacy (Verzeichnis)[\<br
\>\<br /\>]{.underline}

</div>

 

\+

<div>

[Bei dieser Installationsmethode wird weder ein Desktop-Icon noch ein
Eintrag im Startmenü erzeugt und das Starten von YaCy ist nur durch
Aufrufen des Startskripts möglich. Dazu muss die Eingabeaufforderung
unter Startmenü =\> Alle Programme =\> Zubehör =\> Eingabeaufforderung
aufgerufen werden. Dann muss mit \'\'cd
C:\\users\\\<Benutzername\>\\YaCy\'\' in das
YaCy-Installationsverzeichnis gewechselt werden, wobei der Pfad geeignet
anzupassen ist. Nun wird mit \'\'starYACY.bat\'\' das Startskript
aufgerufen.\<br /\>\<br /\>]{.underline}

</div>

 

\+

<div>

[Um YaCy zu deinstallieren, muss ggf. zunächst \[\[De:WinService\|YaCy
als Windows Service\]\] deinstalliert werden. Danach kann das
YaCy-Verzeichnis einfach gelöscht werden.]{.underline}

</div>

 

<div>

\<br /\>\<br /\>\<br /\>\<br /\>

</div>

 

<div>

\<br /\>\<br /\>\<br /\>\<br /\>

</div>

 

 

Zeile 23:

Zeile 26:

 

 

 

<div>

==YaCy als Windows Service==

</div>

 

<div>

==YaCy als Windows Service==

</div>

−

<div>

~~Damit~~ YaCy ~~als~~ Windows ~~Service~~ gestartet werden ~~kann~~,
~~muß YaCy auf einer~~ der ~~lokalen Festplatten installiert werden.
Eine detaillierte Anleitung zur Konfiguration~~ von YaCy als Windows
Service ~~finden Sie~~ \[\[De:WinService\|~~hier~~\]\].\<br /\>

</div>

\+

<div>

[Wenn]{.underline} YaCy [immer beim Booten von]{.underline} Windows
gestartet [und beim Herunterfahren von Windows gestoppt]{.underline}
werden [soll]{.underline}, [muss nach]{.underline} der
[Installation]{.underline} von [YaCy ausserdem]{.underline} YaCy als
Windows Service [installiert werden. Dies erfolgt am einfachsten durch
Aufrufen des Skripts \'\'installYaCyWindwosService.bat\'\'. Alternativ
kann der Windows Service mit]{.underline} \[\[De:WinService\|[dieser
Anleitung]{.underline}\]\] [manuell eingerichtet
werden]{.underline}.\<br /\>

</div>

−

<div>

\<br /\>

</div>

\+

<div>

[Um den Windows Service per Skript einzurichten, muss zunächst die
Eingabeaufforderung unter Startmenü =\> Alle Programme =\> Zubehör =\>
Eingabeaufforderung aufgerufen werden. Dann muss mit \'\'cd
C:\\users\\\<Benutzername\>\\YaCy\'\' in das
YaCy-Installationsverzeichnis gewechselt werden, wobei der Pfad geeignet
anzupassen ist. Nun wird mit \'\'installYaCyWindwosService.bat\'\' das
Skript aufgerufen, das YaCy als Windows Service
installiert.]{.underline} \<br /\>

</div>

 

\+

<div>

[Um YaCy als Windows Service zu testen, muss man vor einem Neustart des
Rechners ggf. \[\[De:FirstStart\#YaCy\_beenden\|YaCy sauber beenden\]\].
Ob YaCy nach dem Neustart automatisch gestartet wurde, kann man durch
Aufrufen des \[http://localhost:8090 YaCy-Web-Interface\] im Browser
testen.]{.underline}

</div>

 

\+

<div>

 

</div>

 

\+

<div>

 

</div>

 

 

 

<div>

==VirtualBox==

</div>

 

<div>

==VirtualBox==

</div>
