En:DebianInstall
================

Date: 2013-03-30 07:01:48

[Installation of YaCy on Debian or Ubuntu: ]{.autocomment}

← Nächstältere Version

Version vom 30. März 2013, 06:01 Uhr

Zeile 4:

Zeile 4:

 

<div>

= Installation of YaCy on Debian or Ubuntu =

</div>

 

<div>

= Installation of YaCy on Debian or Ubuntu =

</div>

 

 

−

<div>

~~It~~ is ~~also possible to load packages~~ using ~~the update-server
at~~:

</div>

\+

<div>

[Installation on Debian-based GNU/Linux operating systems]{.underline}
is [easy]{.underline} using [our Debian repository]{.underline}:

</div>

 

 

 

<div>

  http://debian.yacy.net

</div>

 

<div>

  http://debian.yacy.net

</div>

 

 

−

<div>

To use this server ~~write~~ to /etc/apt/sources.list:

</div>

\+

<div>

To use this server[, copy this]{.underline} to [your]{.underline}
/etc/apt/sources.list [file]{.underline}:

</div>

 

<div>

  \<nowiki\>deb http://debian.yacy.net ./\</nowiki\>

</div>

 

<div>

  \<nowiki\>deb http://debian.yacy.net ./\</nowiki\>

</div>

 

 

−

<div>

~~then~~ you can install YaCy with

</div>

\+

<div>

[Afterwards,]{.underline} you can install YaCy with [the following
commands.  Please note that the repository does not have GPG keys set up
as of March 2013, you will usually see a warning prompt pertaining to
this during installation.]{.underline}

</div>

 

<div>

  apt-get update

</div>

 

<div>

  apt-get update

</div>

 

<div>

  apt-get install yacy

</div>

 

<div>

  apt-get install yacy

</div>

 

 

−

<div>

~~if~~ you don\'t already have the Java JDK installed, you may find that
you need to use this command instead (on Ubuntu 10.04 \[Lucid\],  the
\<tt\>yacy\</tt\> package version 1.0svn8138 does not pull in
\<tt\>openjdk-6-jre\</tt\> appropriately as a dependency):

</div>

\+

<div>

[If]{.underline} you don\'t already have the Java JDK installed, you may
find that you need to use this command instead (on Ubuntu 10.04
\[Lucid\],  the \<tt\>yacy\</tt\> package version 1.0svn8138 does not
pull in \<tt\>openjdk-6-jre\</tt\> appropriately as a dependency):

</div>

 

<div>

  apt-get install openjdk-6-jre-headless yacy

</div>

 

<div>

  apt-get install openjdk-6-jre-headless yacy

</div>

 

 

 

<div>

== Important File Locations ==

</div>

 

<div>

== Important File Locations ==

</div>

−

<div>

After the installation, the yacy application path is ~~at~~

</div>

\+

<div>

After the installation, the yacy application path is[:]{.underline}

</div>

 

<div>

  /usr/share/yacy

</div>

 

<div>

  /usr/share/yacy

</div>

 

 

−

<div>

The DATA-path is ~~at~~

</div>

\+

<div>

The DATA-path is[:]{.underline}

</div>

 

<div>

  /var/lib/yacy

</div>

 

<div>

  /var/lib/yacy

</div>

 

 

 

<div>

The configuration files should be here:

</div>

 

<div>

The configuration files should be here:

</div>

 

<div>

  /etc/yacy/

</div>

 

<div>

  /etc/yacy/

</div>

−

<div>

/etc/yacy/yacy.conf is created using the
/usr/share/yacy/defaults/yacy.init file on first run.

</div>

\+

<div>

/etc/yacy/yacy.conf is created using the
/usr/share/yacy/defaults/yacy.init file on [the]{.underline} first run.

</div>

 

 

 

<div>

The log files should be here:

</div>

 

<div>

The log files should be here:

</div>

Zeile 57:

Zeile 57:

 

<div>

  \# that none of the other crontabs do.

</div>

 

<div>

  \# that none of the other crontabs do.

</div>

 

 

−

<div>

If you want to use ~~a~~ \'\'\'root user\'\'\' crontab in Ubuntu, an
example would be  

</div>

\+

<div>

If you want to use [the]{.underline} \'\'\'root user\'\'\' crontab in
Ubuntu [instead]{.underline}, an example would be[:]{.underline}

</div>

 

<div>

  username\@hostname:\~\$ \'\'\'sudo crontab -e\'\'\'  

</div>

 

<div>

  username\@hostname:\~\$ \'\'\'sudo crontab -e\'\'\'  

</div>

 

<div>

  no crontab for root - using an empty one

</div>

 

<div>

  no crontab for root - using an empty one

</div>

Zeile 69:

Zeile 69:

 

<div>

Then add the following at the end of the file:

</div>

 

<div>

Then add the following at the end of the file:

</div>

 

<div>

  0 6 \* \* \* /usr/bin/apt-get update && /usr/bin/apt-get -y
\--force-yes install yacy

</div>

 

<div>

  0 6 \* \* \* /usr/bin/apt-get update && /usr/bin/apt-get -y
\--force-yes install yacy

</div>

−

<div>

~~There~~ is no user name on the line, and absolute paths are used here
to prevent problems~~.~~

</div>

\+

<div>

[Please note, there]{.underline} is no user name on the line
[above]{.underline}, and absolute [(full)]{.underline} paths are used
here to prevent [binary location]{.underline} problems[!]{.underline}

</div>

 

 

 

<div>

== Next Steps ==

</div>

 

<div>

== Next Steps ==

</div>

−

<div>

After you configured YaCy, you may ~~want~~ also to set a
\[\[En:StaticIP \| static IP\]\] to get a unique IP to your YaCy peer.

</div>

\+

<div>

After you configured YaCy, you may also [want]{.underline} to set a
\[\[En:StaticIP \| static IP\]\] to get a unique IP to your YaCy peer.

</div>

 

 

 

<div>

\[\[Category: Pages in English\]\]

</div>

 

<div>

\[\[Category: Pages in English\]\]

</div>
