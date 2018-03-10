Dev:NetbeansHowTo
=================

Date: 2014-10-09 03:31:53

upd auf Git

← Nächstältere Version

Version vom 9. Oktober 2014, 01:31 Uhr

Zeile 5:

Zeile 5:

 

<div>

Netbeans kann kostenlos von \[http://netbeans.org Netbeans.org\]
heruntergeladen werden. Es stehen mehrere Versionen zur Auswahl, wobei
jede für die Arbeit an YaCy geeignet ist. Wer sich unsicher ist, kann
daher zunächst die kleinste Version auswählen.

</div>

 

<div>

Netbeans kann kostenlos von \[http://netbeans.org Netbeans.org\]
heruntergeladen werden. Es stehen mehrere Versionen zur Auswahl, wobei
jede für die Arbeit an YaCy geeignet ist. Wer sich unsicher ist, kann
daher zunächst die kleinste Version auswählen.

</div>

 

 

−

<div>

~~Neben Netbeans muss Subversion installiert sein~~. Neuere Versionen
von Netbeans sind in der Lage, die für einen Zugriff auf
~~Subversion~~-~~Repisitories~~ notwendige Software bei Bedarf
nachzuinstallieren~~. Subversion kann aber auch von
\[http://subversion.tigris.org/ subversion.tigris.org\] heruntergeladen
werden. Für Windows-Systeme empfiehlt sich
\[http://tortoisesvn.tigris.org/ TortoiseSVN\], das sich sehr gut in den
Windows Explorer integriert~~.

</div>

\+

<div>

[Es empfiehlt sich den jeweils aktuellen Source Code direkt aus dem Git
Repository zu laden]{.underline}. Neuere Versionen von Netbeans sind in
der Lage, die für einen Zugriff auf
[Git]{.underline}-[Repositories]{.underline} notwendige Software bei
Bedarf nachzuinstallieren [(Git Plugin)]{.underline}.

</div>

 

 

−

<div>

Außerdem wird ANT benötigt, das ebenfalls in vielen Linux-Distributionen
enthalten ist oder aber von \[http://ant.apache.org/ ant.apache.org\]
heruntergeladen werden kann.

</div>

\+

<div>

Außerdem wird ANT benötigt, das [in der Netbeans Distribution integriert
ist aber]{.underline} ebenfalls in vielen Linux-Distributionen enthalten
ist oder aber von \[http://ant.apache.org/ ant.apache.org\]
heruntergeladen werden kann.

</div>

 

 

 

<div>

===Projekt einrichten===

</div>

 

<div>

===Projekt einrichten===

</div>

Zeile 17:

Zeile 17:

 

<div>

\[\[Bild:Netbeans6.png\|thumb\|Quellpakete angeben\]\]

</div>

 

<div>

\[\[Bild:Netbeans6.png\|thumb\|Quellpakete angeben\]\]

</div>

 

<div>

\[\[Bild:Netbeans7.png\|thumb\|Das erste Mal kompilieren\]\]

</div>

 

<div>

\[\[Bild:Netbeans7.png\|thumb\|Das erste Mal kompilieren\]\]

</div>

−

<div>

Nach der Installation von Netbeans ~~und Subversion~~ kann Netbeans
gestartet werden. Im Menü \'\'\'Window\'\'\' -
\'\'\'~~Versioning~~\'\'\' muss unter \'\'\'~~Subversion~~\'\'\' der
Punkt \'\'\'~~Checkout~~\...\'\'\' gewählt werden. Im nun erscheinenden
Fenster wird der Benutzer aufgefordert, den Pfad zum ~~Subversion~~
Repository einzugeben.  

</div>

\+

<div>

Nach der Installation von Netbeans kann Netbeans gestartet werden. Im
Menü \'\'\'Window\'\'\' - \'\'\'[Team]{.underline}\'\'\' muss unter
\'\'\'[Git]{.underline}\'\'\' der Punkt
\'\'\'[Clone]{.underline}\...\'\'\' gewählt werden. Im nun erscheinenden
Fenster wird der Benutzer aufgefordert, den Pfad zum [Git]{.underline}
Repository einzugeben.  

</div>

 

 

−

<div>

Sollte ~~statt dieses Fensters eine Aufforderung erscheinen, den Pfad zu
SVN einzugeben, so konnte Netbeans SVN nicht automatisch erkennen.
Gründe hierfür können eine Fehlerhafte SVN-Installation oder eine~~
nicht ~~oder falsch gesetzte Umgebungsvariable sein. Neben der Eingabe
des Pfades~~ zur ~~SVN~~-~~Software kann es helfen,~~ Netbeans ~~oder
den Computer neu zu starten oder SVN neu zu installieren.~~

</div>

\+

<div>

Sollte [Git im Menü]{.underline} nicht zur [Auswahl stehen ist unter
\'\'\'Tools\'\'\']{.underline} - [\'\'\'Plugins\'\'\' das Git Plugin
in]{.underline} Netbeans [nachzuinstallieren]{.underline}

</div>

 

 

−

<div>

Der Pfad zum ~~Subversion~~-Repository (\'\'\'Repository URL\'\'\')
lautet:  

</div>

\+

<div>

Der Pfad zum [Git]{.underline}-Repository (\'\'\'Repository URL\'\'\')
lautet:
\'\'\'https://[gitorious]{.underline}.[org]{.underline}/yacy/[rc1.git]{.underline}\'\'\'

</div>

−

<div>

\'\'\'https://~~svn~~.~~berlios.de/svnroot/repos~~/yacy/~~trunk~~\'\'\'

</div>

\+

<div>

</div>

 

 

 

<div>

Weiter Informationen - auch zu alternativen Übertragungswegen (HTTP,
SSH) - bietet die \[http://developer.berlios.de/svn/?group\_id=3505
BerliOS-Seite\] zum Thema SVN.

</div>

 

<div>

Weiter Informationen - auch zu alternativen Übertragungswegen (HTTP,
SSH) - bietet die \[http://developer.berlios.de/svn/?group\_id=3505
BerliOS-Seite\] zum Thema SVN.

</div>

Zeile 28:

Zeile 27:

 

<div>

In den Feldern \'\'\'User\'\'\' und \'\'\'Password\'\'\' können nun die
entsprechenden Daten eingetragen werden, dies ist aber nicht unbedingt
notwendig, da auch ein anonymer (nur lesender) Zugriff auf das
Repository möglich ist. Werden später Daten in das Repository
eingecheckt, werden die Daten dann von Netbeans erfragt.

</div>

 

<div>

In den Feldern \'\'\'User\'\'\' und \'\'\'Password\'\'\' können nun die
entsprechenden Daten eingetragen werden, dies ist aber nicht unbedingt
notwendig, da auch ein anonymer (nur lesender) Zugriff auf das
Repository möglich ist. Werden später Daten in das Repository
eingecheckt, werden die Daten dann von Netbeans erfragt.

</div>

 

 

−

<div>

~~Nach dem Klick auf \'\'\'Next\'\'\' fragt Netbeans nach, ob das
Zertifikat von BerliOS akzeptiert werden soll. Diese Frage bestätigen
(außer es besteht Grund zum Zweifel an der Authentizität).~~

</div>

 

 

 

 

<div>

Die im sich daraufhin öffnenden Fenster enthaltenen Daten können
übernommen und mit \'\'\'Finish\'\'\' bestätigt werden. Netbeans beginnt
nun, den Quellcode von YaCy herunterzuladen, was in Abhängigkeit von der
Geschwindigkeit des Internetzugangs einige in Anspruch nehmen kann.
Nachdem der Quellcode heruntergeladen wurde, erscheint ein Fenster, in
dem die Art des Projects anzugeben ist. Hier sollte \'\'\'Java Project
with Existing Ant Script\'\'\' bzw. \'\'\'Java Free-Form Project\'\'\'
(ab Netbeans 6.1) gewählt und mit \'\'\'Next\'\'\' bestätigt werden.

</div>

 

<div>

Die im sich daraufhin öffnenden Fenster enthaltenen Daten können
übernommen und mit \'\'\'Finish\'\'\' bestätigt werden. Netbeans beginnt
nun, den Quellcode von YaCy herunterzuladen, was in Abhängigkeit von der
Geschwindigkeit des Internetzugangs einige in Anspruch nehmen kann.
Nachdem der Quellcode heruntergeladen wurde, erscheint ein Fenster, in
dem die Art des Projects anzugeben ist. Hier sollte \'\'\'Java Project
with Existing Ant Script\'\'\' bzw. \'\'\'Java Free-Form Project\'\'\'
(ab Netbeans 6.1) gewählt und mit \'\'\'Next\'\'\' bestätigt werden.

</div>
