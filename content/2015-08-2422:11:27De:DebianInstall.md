De:DebianInstall
================

Date: 2015-08-24 22:11:27

← Nächstältere Version

Version vom 24. August 2015, 20:11 Uhr

(5 dazwischenliegende Versionen von einem Benutzer werden nicht
angezeigt)

Zeile 11:

Zeile 11:

 

<div>

Man kann die Packages über den apt-get install Prozess laden, dazu gibt
es einen Update-Server: http://debian.yacy.net

</div>

 

<div>

Man kann die Packages über den apt-get install Prozess laden, dazu gibt
es einen Update-Server: http://debian.yacy.net

</div>

 

 

−

<div>

Als User root eine ~~eigene~~ source-Datei für YaCy ~~erstellen~~:

</div>

\+

<div>

Als User root eine [neue]{.underline} source-Datei [erstellen, in die
die Adresse]{.underline} für [das]{.underline} YaCy[-Package eingefügt
wird]{.underline}:

</div>

 

<div>

  echo \'deb http://debian.yacy.net ./\' \>\>
/etc/apt/sources.list.d/yacy.list

</div>

 

<div>

  echo \'deb http://debian.yacy.net ./\' \>\>
/etc/apt/sources.list.d/yacy.list

</div>

 

 

−

<div>

~~den Entwickler~~-~~Release-Key~~ installieren über ~~einen~~ der
beiden Möglichkeiten:

</div>

\+

<div>

[Um sicherzustellen, dass ein unverfälschtes YaCy]{.underline}-[Package
heruntergeladen wird, ist das Package mit einem Entwicklerschlüssel
signiert. Diesen muss man zum Abgleich]{.underline} installieren über
[eine]{.underline} der beiden Möglichkeiten:

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

 

 

−

<div>

~~danach~~ kann man YaCy auf Debian installieren mit

</div>

\+

<div>

[Danach]{.underline} kann man YaCy auf Debian installieren mit

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

Das ~~yacy Programmverzeichnis befindet sich~~ dann ~~in~~

</div>

\+

<div>

Das [YACY-HOME-Verzeichnis ist]{.underline} dann

</div>

 

<div>

  /usr/share/yacy

</div>

 

<div>

  /usr/share/yacy

</div>

 

 

Zeile 39:

Zeile 39:

 

<div>

  http://localhost:8090/

</div>

 

<div>

  http://localhost:8090/

</div>

 

 

−

<div>

~~Man kann einen beliebigen Port für das Webinterface in der~~ YaCy
~~Konfiguration einstellen~~, ~~den Port 80 richtet man aber wegen den
notwendigen Administrationsrechten besser über ein \[\[De:Portforwarding
\| Portforwarding\]\] ein.~~

</div>

\+

<div>

[Wenn]{.underline} YaCy [als Debian-Package installiert
wurde]{.underline}, funktioniert der YaCy-interne auto-updater nicht.
Ein Update muss aus der debian Systemumgebung heraus erfolgen,
beispielsweise mit einem cronjob. Dazu in /etc/crontab [folgende Zeile
ergänzen:]{.underline}

</div>

−

<div>

 

</div>

\+

<div>

</div>

−

<div>

~~In dieser Konfiguration~~ funktioniert der YaCy-interne auto-updater
nicht. Ein Update muss aus der debian Systemumgebung heraus erfolgen,
beispielsweise mit einem cronjob. Dazu in /etc/crontab

</div>

\+

<div>

</div>

 

<div>

  0 6 \* \* \* root apt-get update && apt-get -y \--force-yes install
yacy

</div>

 

<div>

  0 6 \* \* \* root apt-get update && apt-get -y \--force-yes install
yacy

</div>

−

<div>

~~hineinschreiben~~

</div>

\+

<div>

 

</div>

 

 

 

 
