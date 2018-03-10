De:VirtualBoxInstall
====================

Date: 2015-11-17 20:58:11

[YaCy in einer VirtualBox installieren: ]{.autocomment}

← Nächstältere Version

Version vom 17. November 2015, 19:58 Uhr

Zeile 1:

Zeile 1:

 

<div>

= YaCy in einer VirtualBox installieren =

</div>

 

<div>

= YaCy in einer VirtualBox installieren =

</div>

 

 

−

<div>

\[https://www.virtualbox.org/ VirtualBox\] ist ein kostenloses Programm
für Windows, Mac OS, Linux und Solaris zur Virtualisierung von Rechnern.
Um YaCy auszuprobieren steht eine virtuelle Maschine, basierend auf
~~debian~~ Linux bereit. Die Installation ist auf allen Betriebssystemen
gleich und sehr einfach:

</div>

\+

<div>

\[https://www.virtualbox.org/ VirtualBox\] ist ein kostenloses Programm
für Windows, Mac OS, Linux und Solaris zur Virtualisierung von Rechnern.
Um YaCy auszuprobieren steht eine virtuelle Maschine, basierend auf
[Debian]{.underline} Linux bereit. Die Installation ist auf allen
Betriebssystemen gleich und sehr einfach:

</div>

 

<div>

\* zunächst VirtualBox von https://www.virtualbox.org/wiki/Downloads für
das eigene Betriebssysten herunterladen und installieren.

</div>

 

<div>

\* zunächst VirtualBox von https://www.virtualbox.org/wiki/Downloads für
das eigene Betriebssysten herunterladen und installieren.

</div>

 

<div>

\* die virtuelle Maschine mit vorinstalliertem YaCy herunterladen von
http://yacy.net/release/yacy-debian-demo.ova

</div>

 

<div>

\* die virtuelle Maschine mit vorinstalliertem YaCy herunterladen von
http://yacy.net/release/yacy-debian-demo.ova

</div>

 

<div>

\* yacy-debian-demo.ova doppelklicken (öffnet dann VirtualBox
automatisch) oder mit VirtualBox im Menüpunkt Datei -\> Appliance
Importieren öffnen.

</div>

 

<div>

\* yacy-debian-demo.ova doppelklicken (öffnet dann VirtualBox
automatisch) oder mit VirtualBox im Menüpunkt Datei -\> Appliance
Importieren öffnen.

</div>

−

<div>

\* die ~~Appliance~~ yacy-debian-demo in VirtualBox starten (markieren
und dann grünen Pfeil klicken)

</div>

\+

<div>

\* die [Anwendung]{.underline} yacy-debian-demo in VirtualBox starten
(markieren und dann grünen Pfeil klicken)

</div>

 

 

−

<div>

Die ~~Appliance~~ bootet dann (startet zunächst ein Debian Linux) und
innerhalb von Debian bootet dann YaCy automatisch. YaCy ist im
Peer-to-Peer Modus und liefert bei Suchanfragen Ergebnisse aus dem
Freeworld-Netz. Man muss hier gar nichts konfigurieren, nur einen Moment
warten. Ist die VM dann vollständig hochgefahren, kann die YaCy
Suchseite aufgerufen werden unter http://192.168.4.4:8090.

</div>

\+

<div>

Die [Anwendung]{.underline} bootet dann (startet zunächst ein Debian
Linux) und innerhalb von Debian bootet dann YaCy automatisch. YaCy ist
im Peer-to-Peer Modus und liefert bei Suchanfragen Ergebnisse aus dem
Freeworld-Netz. Man muss hier gar nichts konfigurieren, nur einen Moment
warten. Ist die VM dann vollständig hochgefahren, kann die YaCy
Suchseite aufgerufen werden unter http://192.168.4.4:8090.

</div>

 

 

 

<div>

== Zugangsdaten ==

</div>

 

<div>

== Zugangsdaten ==

</div>

−

<div>

Die ~~Appliance~~ hat läuft standardmäßig unter der IP 192.168.4.4 und
hat drei Accounts vorkonfiguriert:

</div>

\+

<div>

Die [Anwendung]{.underline} hat läuft standardmäßig unter der IP
192.168.4.4 und hat drei Accounts vorkonfiguriert:

</div>

 

<div>

\* den root-Account des Debian Linux, das Passwort ist \'password\'

</div>

 

<div>

\* den root-Account des Debian Linux, das Passwort ist \'password\'

</div>

 

<div>

\* einen User-Account unter Linux mit Namen \'administrator\', das
Passwort ist \'password\'

</div>

 

<div>

\* einen User-Account unter Linux mit Namen \'administrator\', das
Passwort ist \'password\'

</div>

Zeile 27:

Zeile 27:

 

 

 

<div>

== Resourcenbedarf auf http://yacy.net für den Download ==

</div>

 

<div>

== Resourcenbedarf auf http://yacy.net für den Download ==

</div>

−

<div>

Weil der Download der VirtualBox VM von YaCy wesentlich größer ist (\>
200MB) als das normale Release (ca. 35MB) empfehlen wir diese VM auf
weiteren Wegen als über den Download von yacy.net zu ~~sharen~~ (z.B.
über bittorrent) und bitten hierbei um Mithilfe. \'\'\'Wir bitten
ausserdem, diesen Download, das dafür notwendige Hosting und die dafür
notwendige Bandbreite mit einer Spende über eine der
\[http://yacy.net/include/donate.html Spendenmöglichkeiten\] auf
yacy.net zu unterstützen!\'\'\'

</div>

\+

<div>

Weil der Download der VirtualBox VM von YaCy wesentlich größer ist (\>
200MB) als das normale Release (ca. 35MB) empfehlen wir diese VM auf
weiteren Wegen als über den Download von yacy.net zu
[verteilen]{.underline} (z.B. über bittorrent) und bitten hierbei um
Mithilfe. \'\'\'Wir bitten ausserdem, diesen Download, das dafür
notwendige Hosting und die dafür notwendige Bandbreite mit einer Spende
über eine der \[http://yacy.net/include/donate.html
Spendenmöglichkeiten\] auf yacy.net zu unterstützen!\'\'\'

</div>

 

 

 

<div>

\[\[Kategorie: De:Installation\]\]

</div>

 

<div>

\[\[Kategorie: De:Installation\]\]

</div>

 

<div>

\[\[Kategorie: De:Anleitung\]\]

</div>

 

<div>

\[\[Kategorie: De:Anleitung\]\]

</div>

 

<div>

\[\[Kategorie: Linux\]\]

</div>

 

<div>

\[\[Kategorie: Linux\]\]

</div>
