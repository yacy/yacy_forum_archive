De:VirtualBoxInstall
====================

Date: 2014-09-09 15:46:27

YaCy Demo auf einer VirtualBox

**Neue Seite**

<div>

= YaCy in einer VirtualBox installieren =\
\
\[https://www.virtualbox.org/ VirtualBox\] ist ein kostenloses Programm
für Windows, Mac OS, Linux und Solaris zur Virtualisierung von Rechnern.
Um YaCy auszuprobieren steht eine virtuelle Maschine, basierend auf
debian Linux bereit. Die Installation ist auf allen Betriebssystemen
gleich und sehr einfach:\
\* zunächst VirtualBox von https://www.virtualbox.org/wiki/Downloads für
das eigene Betriebssysten herunterladen und installieren.\
\* die virtuelle Maschine mit vorinstalliertem YaCy herunterladen von
http://yacy.net/release/yacy-debian-demo.ova\
\* yacy-debian-demo.ova doppelklicken (öffnet dann VirtualBox
automatisch) oder mit VirtualBox im Menüpunkt Datei -\> Appliance
Importieren öffnen.\
\* die Appliance yacy-debian-demo in VirtualBox starten (markieren und
dann grünen Pfeil klicken)\
\
Die Appliance bootet dann (startet zunächst ein Debian Linux) und
innerhalb von Debian bootet dann YaCy automatisch. YaCy ist im
Peer-to-Peer Modus und liefert bei Suchanfragen Ergebnisse aus dem
Freeworld-Netz. Man muss hier gar nichts konfigurieren, nur einen Moment
warten. Ist die VM dann vollständig hochgefahren, kann die YaCy
Suchseite aufgerufen werden unter http://192.168.4.4:8090.\
\
== Zugangsdaten ==\
Die Appliance hat läuft standardmäßig unter der IP 192.168.4.4 und hat
drei Accounts vorkonfiguriert:\
\* den root-Account des Debian Linux, das Passwort ist \'password\'\
\* einen User-Account unter Linux mit Namen \'administrator\', das
Passwort ist \'password\'\
\* den YaCy admin-Account mit Account Namen \'admin\' und Passwort
\'password\'\
Es wird empfohlen alle drei Account-Passwörter zu ändern!\
\
== Systemkonfiguration ==\
Die VM wurde mit folgenden Systemeinstellungen konfiguriert:\
\* 2 GB RAM für das Linux, 600MB davon für YaCy\
\* maximal 20GB Plattenplatz\
\* 2 Prozessorcores zugewiesen.\
Diese Einstellungen können leicht über den \'Ändern\'-Knopf in der
VirtualBox Administration geändert werden.\
\
== Resourcenbedarf auf http://yacy.net für den Download ==\
Weil der Download der VirtualBox VM von YaCy wesentlich größer ist (\>
200MB) als das normale Release (ca. 35MB) empfehlen wir diese VM auf
weiteren Wegen als über den Download von yacy.net zu sharen (z.B. über
bittorren) und bitten hierbei um Mithilfe. \'\'\'Wir bitten ausserdem,
diesen Download, das dafür notwendige Hosting und die dafür notwendige
Bandbreite mit einer Spende über eine der Spendenmöglichkeiten auf
yacy.net zu unterstützen!\'\'\'\
\
\[\[Kategorie: De:Installation\]\]\
\[\[Kategorie: De:Anleitung\]\]\
\[\[Kategorie: Linux\]\]

</div>
