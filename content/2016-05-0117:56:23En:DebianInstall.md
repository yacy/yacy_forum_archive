En:DebianInstall
================

Date: 2016-05-01 17:56:23

[Installation of YaCy on Debian: ]{.autocomment}

← Nächstältere Version

Version vom 1. Mai 2016, 15:56 Uhr

(Eine dazwischenliegende Version von einem Benutzer wird nicht
angezeigt)

Zeile 17:

Zeile 17:

 

<div>

  apt-key advanced \--keyserver pgp.net.nz \--recv-keys 03D886E7

</div>

 

<div>

  apt-key advanced \--keyserver pgp.net.nz \--recv-keys 03D886E7

</div>

 

 

−

<div>

And finally install YaCy itself

</div>

\+

<div>

And finally install YaCy itself[.  \'\'\'Warning!\'\'\' If you will be
using Tor, it is important to read
http://www.yacy-websearch.net/wiki/index.php/En:YaCy-Tor before taking
the next step!  Tor must be configured for YaCy before YaCy runs for the
time.  Running \"apt-get install yacy\" before setting up Tor will
create a state for which there is no documentation to recover
from.]{.underline}

</div>

 

<div>

  apt-get update

</div>

 

<div>

  apt-get update

</div>

 

<div>

  apt-get install openjdk-7-jre-headless \# java 7 is sufficient, only a
headless version is needed

</div>

 

<div>

  apt-get install openjdk-7-jre-headless \# java 7 is sufficient, only a
headless version is needed

</div>
