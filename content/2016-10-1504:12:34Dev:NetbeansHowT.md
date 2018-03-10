Dev:NetbeansHowTo
=================

Date: 2016-10-15 04:12:34

Maven Projekt

← Nächstältere Version

Version vom 15. Oktober 2016, 02:12 Uhr

Zeile 38:

Zeile 38:

 

<div>

=== Java 1.7===

</div>

 

<div>

=== Java 1.7===

</div>

 

<div>

Da YaCy auf Java 1.7 basiert, sollte (wenn möglich) das JDK 1.7
installiert werden und zum Kompilieren (zumindest für lokale Tests)
genutzt werden, um versehentliches Benutzen von Java 1.8-features zu
verhindern. Es is möglich, mehrere JDKs parallel zu installieren. In
Netbeans können unter \'\'\'Tools\'\'\' \> \'\'\'Java Platforms\'\'\'
zusätzliche Java-Umgebungen hinzugefügt werden. Um Java 1.7 auch
tatsächlich zum Kompilieren zu nutzen, kann unter \'\'\'Java Sources
Classpath\'\'\' (siehe vorheriger Absatz) die gewünschte Version gewählt
werden.

</div>

 

<div>

Da YaCy auf Java 1.7 basiert, sollte (wenn möglich) das JDK 1.7
installiert werden und zum Kompilieren (zumindest für lokale Tests)
genutzt werden, um versehentliches Benutzen von Java 1.8-features zu
verhindern. Es is möglich, mehrere JDKs parallel zu installieren. In
Netbeans können unter \'\'\'Tools\'\'\' \> \'\'\'Java Platforms\'\'\'
zusätzliche Java-Umgebungen hinzugefügt werden. Um Java 1.7 auch
tatsächlich zum Kompilieren zu nutzen, kann unter \'\'\'Java Sources
Classpath\'\'\' (siehe vorheriger Absatz) die gewünschte Version gewählt
werden.

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[== Netbeans Maven Projekt ==]{.underline}

</div>

 

\+

<div>

[Netbeans unterstützt das Maven Build Tool sehr gut und das YaCy
Git-Repository enthält auch die Konfiguration um YaCy als Maven-Projekt
in Netbeans zu öffnen.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Wenn der Quellcode bereits auf dem eigenen Rechner ist, kann in
Netbeans einfach mit Neues Projekt und nachfolgend mit Auswahl
\'\'\'Maven\'\'\' ein Maven-Projekt direkt geöffnet werden und es sind
keine weiteren Konfigurationen nötig.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Für die erstmalige Verwendung von YaCy als Maven-Projekt muss das
Projekt \'\'\'YaCy Build Library Utility\'\'\' im Unterverzeichnis
\'\'\'libbuild\'\'\' geöffnet und kompiliert werden (dies ist das Maven
Master-Projekt welches alle benötigten Unterprojekte ausführt. Da YaCy
erst nachträglich für Maven konfiguriert wurde (mit vorgegebener
Verzeichnisstruktur) ist das Masterprojekt nicht im Hauptverzeichnis
sondern im Unterverzeichnis libbuild). Nachdem die benötigten Libraries
einmal erstellt wurden kann man direkt mit dem YaCy Search Server
Projekt weiterarbeiten.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Wenn der Quellcode vom Git-Repository geladen werden soll (empfohlen),
dann die Schritte wie oben beschrieben (Projekt einrichten) ausführen
(\'\'\'Team\'\'\' \> \'\'\'Git\'\'\' \> \'\'\'Clone\'\'\')]{.underline}

</div>

 

 

 

<div>

\[\[Category:Dev:Manual\]\]

</div>

 

<div>

\[\[Category:Dev:Manual\]\]

</div>
