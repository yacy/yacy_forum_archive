En:DebianInstall
================

Date: 2013-12-18 00:24:46

[Direct editing of /etc/apt/sources.list got deprecated. Added developer
key install information. Shortened the openjdk stuff: ]{.autocomment}

← Nächstältere Version

Version vom 17. Dezember 2013, 23:24 Uhr

Zeile 2:

Zeile 2:

 

<div>

{{interwikiES\|Es:Instalación en Debian}}

</div>

 

<div>

{{interwikiES\|Es:Instalación en Debian}}

</div>

 

<div>

{{interwikiFR\|Fr:DebianInstall}}

</div>

 

<div>

{{interwikiFR\|Fr:DebianInstall}}

</div>

−

<div>

= Installation of YaCy on Debian ~~or Ubuntu~~ =

</div>

\+

<div>

= Installation of YaCy on Debian =

</div>

 

 

 

<div>

Installation on Debian-based GNU/Linux operating systems is easy using
our Debian repository:

</div>

 

<div>

Installation on Debian-based GNU/Linux operating systems is easy using
our Debian repository:

</div>

Zeile 8:

Zeile 8:

 

<div>

  http://debian.yacy.net

</div>

 

<div>

  http://debian.yacy.net

</div>

 

 

−

<div>

~~To use this server, copy this to your~~ /etc/apt/sources.list file:

</div>

\+

<div>

[Because direct editing of]{.underline} /etc/apt/sources.list [became
depricated create a new]{.underline} file:

</div>

−

<div>

  ~~\<nowiki\>deb http:~~//~~debian~~.~~yacy.net~~ ./~~\</nowiki\>~~

</div>

\+

<div>

  [touch]{.underline}
/[etc]{.underline}/[apt/sources]{.underline}.[list]{.underline}.[d]{.underline}/[yacy.list]{.underline}

</div>

 

 

−

<div>

~~Afterwards, you can install YaCy with~~ the ~~following commands.~~
~~Please note that~~ the ~~repository does not have GPG keys set up as~~
of ~~March 2013, you will usually see a warning prompt pertaining to
this during installation~~.

</div>

\+

<div>

[And insert into this file]{.underline} the [neccessary
information]{.underline}

</div>

 

\+

<div>

  [echo \'deb http://debian.yacy.net ./\' \>
/etc/apt/sources.list.d/yacy.list]{.underline}

</div>

 

\+

<div>

 

</div>

 

\+

<div>

[Install]{.underline} the [developer key with one]{.underline} of [the
two next methods]{.underline}

</div>

 

\+

<div>

[wget http://debian]{.underline}.[yacy.net/yacy\_orbiter\_key.asc -O- \|
apt-key add -]{.underline}

</div>

 

\+

<div>

[apt-key advanced \--keyserver pgp.net.nz \--recv-keys
03D886E7]{.underline}

</div>

 

\+

<div>

 

</div>

 

\+

<div>

[And finally install YaCy itself]{.underline}

</div>

 

<div>

  apt-get update

</div>

 

<div>

  apt-get update

</div>

 

\+

<div>

[apt-get install openjdk-6-jre \# just if openjdk-6-jre or
openjdk-6-jre-headless isn\'t installed]{.underline}

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

 

−

<div>

~~If you don\'t already have the Java JDK installed, you may find that
you need to use this command instead (on Ubuntu 10.04 \[Lucid\],  the
\<tt\>yacy\</tt\> package version 1.0svn8138 does not pull in
\<tt\>openjdk-6-jre\</tt\> appropriately as a dependency):~~

</div>

 

−

<div>

~~apt-get install openjdk-6-jre-headless yacy~~

</div>

 

 

 

 

<div>

== Important File Locations ==

</div>

 

<div>

== Important File Locations ==

</div>
