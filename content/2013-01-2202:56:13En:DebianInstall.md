En:DebianInstall
================

Date: 2013-01-22 02:56:13

[Installation of YaCy on Debian or Ubuntu: ]{.autocomment} only the
headless version is needed

← Nächstältere Version

Version vom 22. Januar 2013, 01:56 Uhr

Zeile 16:

Zeile 16:

 

 

 

<div>

if you don\'t already have the Java JDK installed, you may find that you
need to use this command instead (on Ubuntu 10.04 \[Lucid\],  the
\<tt\>yacy\</tt\> package version 1.0svn8138 does not pull in
\<tt\>openjdk-6-jre\</tt\> appropriately as a dependency):

</div>

 

<div>

if you don\'t already have the Java JDK installed, you may find that you
need to use this command instead (on Ubuntu 10.04 \[Lucid\],  the
\<tt\>yacy\</tt\> package version 1.0svn8138 does not pull in
\<tt\>openjdk-6-jre\</tt\> appropriately as a dependency):

</div>

−

<div>

  apt-get install ~~yacy~~ openjdk-6-jre

</div>

\+

<div>

  apt-get install openjdk-6-jre[-headless yacy]{.underline}

</div>

 

 

 

<div>

After the installation, the yacy application path is at

</div>

 

<div>

After the installation, the yacy application path is at

</div>
