De:DebianInstall
================

Date: 2014-06-09 15:50:28

[YaCy unter Debian installieren: ]{.autocomment}

← Nächstältere Version

Version vom 9. Juni 2014, 13:50 Uhr

Zeile 17:

Zeile 17:

 

<div>

danach kann man YaCy auf Debian installieren mit

</div>

 

<div>

danach kann man YaCy auf Debian installieren mit

</div>

 

<div>

  apt-get update

</div>

 

<div>

  apt-get update

</div>

−

<div>

  apt-get install openjdk-~~6~~-jre \# ~~benötigt falls noch nicht
installiert~~

</div>

\+

<div>

  apt-get install openjdk-[7]{.underline}-jre[-headless]{.underline} \#
[die headless Java Version reicht aus]{.underline}

</div>

 

<div>

  apt-get install yacy

</div>

 

<div>

  apt-get install yacy

</div>

 

 
