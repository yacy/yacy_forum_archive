De:DebianInstall
================

Date: 2015-11-25 22:57:04

← Nächstältere Version

Version vom 25. November 2015, 21:57 Uhr

Zeile 1:

Zeile 1:

−

<div>

~~{{interwikiDE\|De:DebianInstall}}~~

</div>

 

−

<div>

~~{{interwikiEN\|En:DebianInstall}}~~

</div>

 

−

<div>

~~{{interwikiRU\|Ru:Debian Установка}}~~

</div>

 

−

<div>

~~{{interwikiFR\|Fr:DebianInstall}}~~

</div>

 

−

<div>

~~{{interwikiES\|Es:Instalación en Debian}}~~

</div>

 

−

<div>

</div>

 

 

<div>

= YaCy unter Debian installieren =

</div>

 

<div>

= YaCy unter Debian installieren =

</div>

 

 

Zeile 23:

Zeile 17:

 

<div>

  apt-get install yacy

</div>

 

<div>

  apt-get install yacy

</div>

 

 

−

<div>

Das ~~YACY~~-HOME-Verzeichnis ist dann

</div>

\+

<div>

Das [YaCy]{.underline}-HOME-Verzeichnis ist dann

</div>

 

<div>

  /usr/share/yacy

</div>

 

<div>

  /usr/share/yacy

</div>

 

 

−

<div>

Das Datenverzeichnis DATA befindet sich ~~in~~

</div>

\+

<div>

Das Datenverzeichnis DATA befindet sich [im
YaCy-Home-Verzeichnis.]{.underline}

</div>

−

<div>

~~/var/lib/yacy~~

</div>

\+

<div>

 

</div>

 

 

 

<div>

YaCy wird dann bei einem Debian-Startup automatisch gestartet, und bei
einem Shutdown auch beendet.

</div>

 

<div>

YaCy wird dann bei einem Debian-Startup automatisch gestartet, und bei
einem Shutdown auch beendet.

</div>

Zeile 41:

Zeile 35:

 

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

−

<div>

 

</div>

\+

<div>

[\<br /\>]{.underline}

</div>

 

\+

<div>

[{{interwikiDE\|De:DebianInstall}}]{.underline}

</div>

 

\+

<div>

[{{interwikiEN\|En:DebianInstall}}]{.underline}

</div>

 

\+

<div>

[{{interwikiRU\|Ru:Debian Установка}}]{.underline}

</div>

 

\+

<div>

[{{interwikiFR\|Fr:DebianInstall}}]{.underline}

</div>

 

\+

<div>

[{{interwikiES\|Es:Instalación en Debian}}]{.underline}

</div>

 

 

 

 
