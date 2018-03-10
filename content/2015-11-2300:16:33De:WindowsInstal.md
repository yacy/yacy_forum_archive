De:WindowsInstall
=================

Date: 2015-11-23 00:16:33

← Nächstältere Version

Version vom 22. November 2015, 23:16 Uhr

Zeile 6:

Zeile 6:

 

<div>

Der Windows-Installer steht auf der \[http://yacy.net YaCy-Seite\] zum
Download zur Verfügung (siehe Abbildung). Damit kann YaCy auf dem unter
Windows üblichen Weg mit einer .exe-Datei installiert werden.\<br
/\>\<br /\>

</div>

 

<div>

Der Windows-Installer steht auf der \[http://yacy.net YaCy-Seite\] zum
Download zur Verfügung (siehe Abbildung). Damit kann YaCy auf dem unter
Windows üblichen Weg mit einer .exe-Datei installiert werden.\<br
/\>\<br /\>

</div>

 

<div>

Bei der Installation wird überprüft, ob die benötigte
Java-Laufzeitumgebung bereits installiert ist. Ist dies nicht der Fall,
wird diese automatisch nachgeladen und installiert. Sollten für die
Installation von YaCy keine Administrator-Rechte vorliegen, wird die
Java-Installation in den Ordner \"Gemeinsame Dokumente\" (XP) bzw.
\"Öffentliche Dokumente\" (Vista) abgelegt. Von dort kann dann ein
Administrator Java auf dem System installieren. Um dies zu vermeiden,
kann die yacy\_\<version\>.exe mit Administratorrechten ausgeführt
werden.\<br /\>\<br /\>

</div>

 

<div>

Bei der Installation wird überprüft, ob die benötigte
Java-Laufzeitumgebung bereits installiert ist. Ist dies nicht der Fall,
wird diese automatisch nachgeladen und installiert. Sollten für die
Installation von YaCy keine Administrator-Rechte vorliegen, wird die
Java-Installation in den Ordner \"Gemeinsame Dokumente\" (XP) bzw.
\"Öffentliche Dokumente\" (Vista) abgelegt. Von dort kann dann ein
Administrator Java auf dem System installieren. Um dies zu vermeiden,
kann die yacy\_\<version\>.exe mit Administratorrechten ausgeführt
werden.\<br /\>\<br /\>

</div>

−

<div>

YaCy wird standardmäßg in das Verzeichnis
C:\\users\\\<Benutzername\>\\YaCy installiert. Wenn bei der Installation
manuell ein Installationspfad ausgewählt wird, der nicht innnerhalb von
C:\\users\\\<Benutzername\> liegt, sind zum Starten von YaCy ggf.
Administratorrechte nötig, wovon abzuraten ist. Bei der Installation
werden auf dem ~~Deskop~~ ein YaCy-Icon und im Startmenü ein
YaCy-Eintrag angelegt, mit denen man \[\[De:~~FirstStart~~\|YaCy
starten\]\] kann.\<br /\>\<br /\>

</div>

\+

<div>

YaCy wird standardmäßg in das Verzeichnis
C:\\users\\\<Benutzername\>\\YaCy installiert. Wenn bei der Installation
manuell ein Installationspfad ausgewählt wird, der nicht innnerhalb von
C:\\users\\\<Benutzername\> liegt, sind zum Starten von YaCy ggf.
Administratorrechte nötig, wovon abzuraten ist. Bei der Installation
werden auf dem [Desktop]{.underline} ein YaCy-Icon und im Startmenü ein
YaCy-Eintrag angelegt, mit denen man \[\[De:[Startup]{.underline}\|YaCy
starten\]\] kann.\<br /\>\<br /\>

</div>

−

<div>

Um YaCy zu deinstallieren, muss ggf. zunächst
\[\[De:~~WindowsInstall\#YaCy als Windows~~ Service\|YaCy als Windows
Service\]\] ~~deinstalliert~~ werden. Danach kann YaCy über das
Startmenü ~~=~~\> Alle Programme ~~=~~\> YaCy ~~=~~\> Uninstall
deinstalliert werden.  

</div>

\+

<div>

Um YaCy zu deinstallieren, muss ggf. zunächst \[\[De:Service\|YaCy als
Windows Service\]\] [deaktiviert]{.underline} werden. Danach kann YaCy
über das Startmenü [-]{.underline}\> Alle Programme [-]{.underline}\>
YaCy [-]{.underline}\> Uninstall deinstalliert werden.  

</div>

 

 

 

<div>

\<br /\>\<br /\>

</div>

 

<div>

\<br /\>\<br /\>

</div>

Zeile 16:

Zeile 16:

 

<div>

Zum Entpacken muss ein geeignetes Programm installiert sein (z.B.
\[http://www.7-zip.org 7zip\],FilZip, WinZip oder WinRAR). Das Archiv
(Dateiendung .tar.gz) kann in ein geeignetes Verzeichnis unterhalb von
C:\\users\\\<Benutzername\> kopiert werden, um es dann mit Rechtsklick
und \"hier entpacken\" zu entpacken. Ggf. wird es im ersten Schritt nur
dekomprimiert und man erhält eine Archiv-Datei (Dateiendung .tar). Diese
Archiv-Datei muss erneut entpackt werden, um das yacy-Verzeicnhis zu
extrahieren.\<br /\>

</div>

 

<div>

Zum Entpacken muss ein geeignetes Programm installiert sein (z.B.
\[http://www.7-zip.org 7zip\],FilZip, WinZip oder WinRAR). Das Archiv
(Dateiendung .tar.gz) kann in ein geeignetes Verzeichnis unterhalb von
C:\\users\\\<Benutzername\> kopiert werden, um es dann mit Rechtsklick
und \"hier entpacken\" zu entpacken. Ggf. wird es im ersten Schritt nur
dekomprimiert und man erhält eine Archiv-Datei (Dateiendung .tar). Diese
Archiv-Datei muss erneut entpackt werden, um das yacy-Verzeicnhis zu
extrahieren.\<br /\>

</div>

 

<div>

Beispiel: yacy\_v1.82.tar.gz (komprimiertes Archiv) =\> entpacken =\>
yacy\_v1.82.tar (Archiv-Datei)=\> entpacken =\> yacy (Verzeichnis)\<br
\>\<br /\>

</div>

 

<div>

Beispiel: yacy\_v1.82.tar.gz (komprimiertes Archiv) =\> entpacken =\>
yacy\_v1.82.tar (Archiv-Datei)=\> entpacken =\> yacy (Verzeichnis)\<br
\>\<br /\>

</div>

−

<div>

Bei dieser Installationsmethode wird weder ein Desktop-Icon noch ein
Eintrag im Startmenü erzeugt und das Starten von YaCy ist nur durch
Aufrufen des Startskripts möglich. Dazu muss die Eingabeaufforderung
unter Startmenü ~~=~~\> Alle Programme ~~=~~\> Zubehör ~~=\>
Eingabeaufforderung~~ aufgerufen werden. Dann muss mit ~~\'\'~~cd
C:\\users\\\<Benutzername\>\\YaCy~~\'\'~~ in das
YaCy-Installationsverzeichnis gewechselt werden, wobei der Pfad geeignet
anzupassen ist. Nun wird mit ~~\'\'starYACY~~.bat~~\'\'~~ das
Startskript aufgerufen.\<br /\>\<br /\>

</div>

\+

<div>

Bei dieser Installationsmethode wird weder ein Desktop-Icon noch ein
Eintrag im Startmenü erzeugt und das Starten von YaCy ist nur durch
Aufrufen des Startskripts möglich. Dazu muss die Eingabeaufforderung
[(]{.underline}unter Startmenü [-]{.underline}\> Alle Programme
[-]{.underline}\> Zubehör[)]{.underline} aufgerufen werden. Dann muss
mit [\<code\>]{.underline}cd
C:\\users\\\<Benutzername\>\\YaCy[\</code\>]{.underline} in das
YaCy-Installationsverzeichnis gewechselt werden, wobei der Pfad geeignet
anzupassen ist. Nun wird mit
[\<code\>startYACY]{.underline}.bat[\</code\>]{.underline} das
Startskript aufgerufen.\<br /\>\<br /\>

</div>

−

<div>

Um YaCy zu deinstallieren, muss ggf. zunächst
\[\[De:~~WinService~~\|YaCy als Windows Service\]\] ~~deinstalliert~~
werden. Danach kann das YaCy-Verzeichnis einfach gelöscht werden.  

</div>

\+

<div>

Um YaCy zu deinstallieren, muss ggf. zunächst
\[\[De:[Service]{.underline}\|YaCy als Windows Service\]\]
[abgemeldet]{.underline} werden. Danach kann das YaCy-Verzeichnis
einfach gelöscht werden.  

</div>

 

<div>

\<br /\>\<br /\>\<br /\>\<br /\>

</div>

 

<div>

\<br /\>\<br /\>\<br /\>\<br /\>

</div>

−

<div>

</div>

 

−

<div>

~~==Firewall freischalten==~~

</div>

 

−

<div>

~~\[\[Bild:Windows-Firewall-Hinweis.png\|thumb\]\]~~

</div>

 

−

<div>

~~Für den Betrieb von YaCy muss der Java-Prozess in der Windows-Firewall
freigegeben werden. Der Windows-Sicherheitshinweis (siehe Abbildung)
wird automatisch beim \[\[De:FirstStart\|ersten Start\]\] von YaCy
angezeigt. Klicken Sie auf die Schaltfläche \"Zugriff zulassen\", um die
Firewall für den Java-Prozess frei zu schalten. \<br /\>\<br /\>\<br
/\>\<br /\>~~

</div>

 

−

<div>

~~\<br /\>~~

</div>

 

−

<div>

</div>

 

−

<div>

~~==YaCy als Windows Service==~~

</div>

 

−

<div>

~~Wenn YaCy immer beim Booten von Windows gestartet und beim
Herunterfahren von Windows gestoppt werden soll, muss nach der
Installation von YaCy ausserdem YaCy als Windows Service installiert
werden. Dies erfolgt am einfachsten durch Aufrufen des Skripts
\'\'installYaCyWindwosService.bat\'\'. Alternativ kann der Windows
Service mit \[\[De:WinService\|dieser Anleitung\]\] manuell eingerichtet
werden.\<br /\>~~

</div>

 

−

<div>

~~Um den Windows Service per Skript einzurichten, muss zunächst die
Eingabeaufforderung unter Startmenü =\> Alle Programme =\> Zubehör =\>
Eingabeaufforderung aufgerufen werden. Dann muss mit \'\'cd
C:\\users\\\<Benutzername\>\\YaCy\'\' in das
YaCy-Installationsverzeichnis gewechselt werden, wobei der Pfad geeignet
anzupassen ist. Nun wird mit \'\'installYaCyWindwosService.bat\'\' das
Skript aufgerufen, das YaCy als Windows Service installiert. \<br /\>~~

</div>

 

−

<div>

~~Um YaCy als Windows Service zu testen, muss man vor einem Neustart des
Rechners ggf. \[\[De:FirstStart\#YaCy\_beenden\|YaCy sauber beenden\]\].
Ob YaCy nach dem Neustart automatisch gestartet wurde, kann man durch
Aufrufen des \[http://localhost:8090 YaCy-Web-Interface\] im Browser
testen.~~

</div>

 

−

<div>

</div>

 

−

<div>

</div>

 

 

 

 

<div>

==VirtualBox==

</div>

 

<div>

==VirtualBox==

</div>
