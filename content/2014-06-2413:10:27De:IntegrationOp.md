De:IntegrationOpera
===================

Date: 2014-06-24 13:10:27

corrected port 8080-\>8090

← Nächstältere Version

Version vom 24. Juni 2014, 11:10 Uhr

Zeile 9:

Zeile 9:

 

<div>

\*Name: YaCy

</div>

 

<div>

\*Name: YaCy

</div>

 

<div>

\*Shortcut: y (Mittels dieser Abkürzung kann man später direkt im
Adressfeld des Browsers suchen.)

</div>

 

<div>

\*Shortcut: y (Mittels dieser Abkürzung kann man später direkt im
Adressfeld des Browsers suchen.)

</div>

−

<div>

\*URL:  http://localhost:~~8080~~/yacysearch.html?search=%s (Die Adresse
und der Port müssen gegebenenfalls angepasst werden, wenn YaCy nicht auf
dm gleichen Rechner läuft wie der Browser oder der Port geändert wurde.)

</div>

\+

<div>

\*URL:  http://localhost:[8090]{.underline}/yacysearch.html?search=%s
(Die Adresse und der Port müssen gegebenenfalls angepasst werden, wenn
YaCy nicht auf dm gleichen Rechner läuft wie der Browser oder der Port
geändert wurde.)

</div>

 

<div>

Nach der Bestätigung der Eingabe kann nun mittels Eingabe von \'\'\'y
suchbegriff\'\'\' im Adressfeld des Browsers suchen.

</div>

 

<div>

Nach der Bestätigung der Eingabe kann nun mittels Eingabe von \'\'\'y
suchbegriff\'\'\' im Adressfeld des Browsers suchen.

</div>

 

 

Zeile 18:

Zeile 18:

 

<div>

  \[Search Engine X\]

</div>

 

<div>

  \[Search Engine X\]

</div>

 

<div>

  Name=&YACY

</div>

 

<div>

  Name=&YACY

</div>

−

<div>

  URL=http://localhost:~~8080~~/yacysearch.html?search=%s&Enter=Search

</div>

\+

<div>

 
URL=http://localhost:[8090]{.underline}/yacysearch.html?search=%s&Enter=Search

</div>

 

<div>

  Query=

</div>

 

<div>

  Query=

</div>

 

<div>

  Key=p

</div>

 

<div>

  Key=p

</div>

Zeile 34:

Zeile 34:

 

<div>

YaCy kann in die Sidebar von Opera integriert werden. Dadurch kann man
YaCy immer bequem neben den eigentlichen Inhalten geöffnet haben und für
die Suche verwenden.

</div>

 

<div>

YaCy kann in die Sidebar von Opera integriert werden. Dadurch kann man
YaCy immer bequem neben den eigentlichen Inhalten geöffnet haben und für
die Suche verwenden.

</div>

 

 

−

<div>

Dazu öffnet man mit \'\'\'Strg + D\'\'\' das Menü zum Hinzufügen eines
neuen Bookmarks. In diesem Menü wählt man \'\'\'Details\'\'\', um eine
Ansicht zu erhalten, in der zusätzliche Parameter angegeben werden
können. Hier Trägt man nun einen Namen und die Adresse des Peers (z.B.
\[http://localhost:~~8080~~/?display=2
http://localhost:~~8080~~/?display=2\]) ein. Außerdem muss ein Haken
neben \'\'\'Show in panel\'\'\' gesetzt werden und mit \'\'\'OK\'\'\'
bestätigt werden (siehe Screenshot).

</div>

\+

<div>

Dazu öffnet man mit \'\'\'Strg + D\'\'\' das Menü zum Hinzufügen eines
neuen Bookmarks. In diesem Menü wählt man \'\'\'Details\'\'\', um eine
Ansicht zu erhalten, in der zusätzliche Parameter angegeben werden
können. Hier Trägt man nun einen Namen und die Adresse des Peers (z.B.
\[http://localhost:[8090]{.underline}/?display=2
http://localhost:[8090]{.underline}/?display=2\]) ein. Außerdem muss ein
Haken neben \'\'\'Show in panel\'\'\' gesetzt werden und mit
\'\'\'OK\'\'\' bestätigt werden (siehe Screenshot).

</div>

 

 

 

<div>

\[\[Bild:Yacyoperasidebar2.png\|thumb\|Opera mit YaCy in der
Sidebar\]\]Wenn die Sidebar noch nicht geöffnet ist, kann dies mit einem
Druck auf \'\'\'F4\'\'\' getan werden. YaCy sollte nun über das oberste
Icon erreichbar sein.

</div>

 

<div>

\[\[Bild:Yacyoperasidebar2.png\|thumb\|Opera mit YaCy in der
Sidebar\]\]Wenn die Sidebar noch nicht geöffnet ist, kann dies mit einem
Druck auf \'\'\'F4\'\'\' getan werden. YaCy sollte nun über das oberste
Icon erreichbar sein.

</div>
