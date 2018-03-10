De:DebianInstall
================

Date: 2015-11-26 02:31:39

← Nächstältere Version

Version vom 26. November 2015, 01:31 Uhr

Zeile 3:

Zeile 3:

 

<div>

Eine Anleitung zum Selberbauen des Debianpaketes
\[\[DebianPaketBauen\|hier\]\].

</div>

 

<div>

Eine Anleitung zum Selberbauen des Debianpaketes
\[\[DebianPaketBauen\|hier\]\].

</div>

 

 

−

<div>

Man kann die Packages über den apt-get install Prozess laden, dazu gibt
es einen ~~Update-Server:~~ http://debian.yacy.net

</div>

\+

<div>

[==Source-Datei einrichten==]{.underline}

</div>

−

<div>

 

</div>

\+

<div>

Man kann die Packages über den apt-get install Prozess laden, dazu gibt
es einen [\[\[]{.underline}http://debian.yacy.net [Update-Server\]\],
den man am besten in]{.underline} eine [neu zu erstellende]{.underline}
source-Datei [einträgt]{.underline}:

</div>

−

<div>

~~Als User root~~ eine ~~neue~~ source-Datei ~~erstellen, in die die
Adresse für das YaCy-Package eingefügt wird~~:

</div>

\+

<div>

</div>

 

<div>

  echo \'deb http://debian.yacy.net ./\' \>\>
/etc/apt/sources.list.d/yacy.list

</div>

 

<div>

  echo \'deb http://debian.yacy.net ./\' \>\>
/etc/apt/sources.list.d/yacy.list

</div>

 

\+

<div>

[\<br /\>]{.underline}

</div>

 

 

 

\+

<div>

[==Entwicklerschlüssel importieren==]{.underline}

</div>

 

<div>

Um sicherzustellen, dass ein unverfälschtes YaCy-Package heruntergeladen
wird, ist das Package mit einem Entwicklerschlüssel signiert. Diesen
muss man zum Abgleich installieren über eine der beiden Möglichkeiten:

</div>

 

<div>

Um sicherzustellen, dass ein unverfälschtes YaCy-Package heruntergeladen
wird, ist das Package mit einem Entwicklerschlüssel signiert. Diesen
muss man zum Abgleich installieren über eine der beiden Möglichkeiten:

</div>

 

<div>

  wget http://debian.yacy.net/yacy\_orbiter\_key.asc -O- \| apt-key add
-

</div>

 

<div>

  wget http://debian.yacy.net/yacy\_orbiter\_key.asc -O- \| apt-key add
-

</div>

 

<div>

  apt-key advanced \--keyserver pgp.net.nz \--recv-keys 03D886E7

</div>

 

<div>

  apt-key advanced \--keyserver pgp.net.nz \--recv-keys 03D886E7

</div>

 

\+

<div>

[\<br /\>]{.underline}

</div>

 

 

 

\+

<div>

[==YaCy installieren==]{.underline}

</div>

 

<div>

Danach kann man YaCy auf Debian installieren mit

</div>

 

<div>

Danach kann man YaCy auf Debian installieren mit

</div>

 

<div>

  apt-get update

</div>

 

<div>

  apt-get update

</div>

 

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

−

<div>

 

</div>

\+

<div>

YaCy [wird bei der Installation als Dienst in]{.underline}
/[etc]{.underline}/[init]{.underline}.[d eingetragen, so
dass]{.underline} YaCy bei einem Debian-Startup automatisch gestartet,
und bei einem Shutdown auch beendet [wird]{.underline}.[\<br
/\>]{.underline}

</div>

−

<div>

~~Das~~ YaCy~~-HOME-Verzeichnis ist dann~~

</div>

\+

<div>

</div>

−

<div>

 /~~usr~~/~~share/yacy~~

</div>

\+

<div>

</div>

−

<div>

 

</div>

\+

<div>

</div>

−

<div>

~~Das Datenverzeichnis DATA befindet sich im YaCy-Home-Verzeichnis~~.

</div>

\+

<div>

</div>

−

<div>

 

</div>

\+

<div>

</div>

−

<div>

 

</div>

\+

<div>

</div>

−

<div>

YaCy ~~wird dann~~ bei einem Debian-Startup automatisch gestartet, und
bei einem Shutdown auch beendet.

</div>

\+

<div>

</div>

−

<div>

 

</div>

\+

<div>

</div>

 

<div>

Man kann YaCy auch manuell starten, stoppen und neustarten:

</div>

 

<div>

Man kann YaCy auch manuell starten, stoppen und neustarten:

</div>

 

<div>

  /etc/init.d/yacy stop

</div>

 

<div>

  /etc/init.d/yacy stop

</div>

 

<div>

  /etc/init.d/yacy start

</div>

 

<div>

  /etc/init.d/yacy start

</div>

 

<div>

  /etc/init.d/yacy restart

</div>

 

<div>

  /etc/init.d/yacy restart

</div>

 

\+

<div>

[\<br /\>]{.underline}

</div>

 

 

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[==YaCy-Web-Interface aufrufen==]{.underline}

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

 

\+

<div>

[\<br /\>]{.underline}

</div>

 

 

 

\+

<div>

[Das YaCy-HOME-Verzeichnis ist dann /usr/share/yacy]{.underline}

</div>

 

\+

<div>

[Das Datenverzeichnis DATA befindet sich im
YaCy-Home-Verzeichnis.]{.underline}

</div>

 

\+

<div>

[\<br /\>]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[==YaCy updaten==]{.underline}

</div>

 

<div>

Wenn YaCy als Debian-Package installiert wurde, funktioniert der
YaCy-interne auto-updater nicht. Ein Update muss aus der debian
Systemumgebung heraus erfolgen, beispielsweise mit einem cronjob. Dazu
in /etc/crontab folgende Zeile ergänzen:

</div>

 

<div>

Wenn YaCy als Debian-Package installiert wurde, funktioniert der
YaCy-interne auto-updater nicht. Ein Update muss aus der debian
Systemumgebung heraus erfolgen, beispielsweise mit einem cronjob. Dazu
in /etc/crontab folgende Zeile ergänzen:

</div>

 

<div>

  0 6 \* \* \* root apt-get update && apt-get -y \--force-yes install
yacy

</div>

 

<div>

  0 6 \* \* \* root apt-get update && apt-get -y \--force-yes install
yacy

</div>

 

\+

<div>

[\<br /\>]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[==YaCy deintstallieren==]{.underline}

</div>

 

\+

<div>

[Wenn bei der Deinstallion auch der Eintrag des YaCy-Dienstes in 
/etc/init.d entfernt werden soll, ist folgende Vorgehensweise zu
empfehlen:]{.underline}

</div>

 

\+

<div>

[apt-get purge yacy]{.underline}

</div>

 

<div>

\<br /\>

</div>

 

<div>

\<br /\>

</div>

 

<div>

{{interwikiDE\|De:DebianInstall}}

</div>

 

<div>

{{interwikiDE\|De:DebianInstall}}

</div>
