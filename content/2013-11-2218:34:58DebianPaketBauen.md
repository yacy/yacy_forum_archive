DebianPaketBauen
================

Date: 2013-11-22 18:34:58

[Debianpaket selbst bauen: ]{.autocomment}

← Nächstältere Version

Version vom 22. November 2013, 17:34 Uhr

Zeile 1:

Zeile 1:

 

<div>

== Debianpaket selbst bauen ==

</div>

 

<div>

== Debianpaket selbst bauen ==

</div>

 

\+

<div>

[Zuvor: die Paketerstellung sollte möglichst von Sicherheitsüberlegungen
aus betrachtet NICHT auf produktiven Servern stattfinden, da eine
umfangreiche Entwicklungsumgebung von Software installiert wird, die bei
einem Einbruch sofort zur Verfügung stünde. Es ist besser, eine
Virtuelle Maschine dafür zu benutzen.]{.underline}

</div>

 

 

−

<div>

~~Zuerst ist~~ ein GIT-Clone ~~machen~~:

</div>

\+

<div>

[Am besten]{.underline} ein [aussagekräftiges Verzeichnis unter
/usr/src/anlegen und dort hingehen:]{.underline}

</div>

 

\+

<div>

[\<pre\>]{.underline}

</div>

 

\+

<div>

[mkdir  /usr/local/src/yacy-git]{.underline}

</div>

 

\+

<div>

[cd /usr/local/src/yacy-git]{.underline}

</div>

 

\+

<div>

[\</pre\>]{.underline}

</div>

 

\+

<div>

 

</div>

 

\+

<div>

[Dann einen]{.underline} GIT-Clone [erstellen]{.underline}:

</div>

 

<div>

\<pre\>

</div>

 

<div>

\<pre\>

</div>

 

<div>

git clone git://gitorious.org/yacy/rc1.git

</div>

 

<div>

git clone git://gitorious.org/yacy/rc1.git

</div>

 

<div>

\</pre\>

</div>

 

<div>

\</pre\>

</div>

 

 

−

<div>

Dann ~~ein Pakete~~ nachinstallieren:

</div>

\+

<div>

Dann [in das Unterzeichnis rc1 gehen]{.underline}

</div>

 

\+

<div>

[\<pre\>]{.underline}

</div>

 

\+

<div>

[cd rc1]{.underline}

</div>

 

\+

<div>

[\</pre\>]{.underline}

</div>

 

\+

<div>

 

</div>

 

\+

<div>

[Dann notwendige Kompilierungspakete]{.underline} nachinstallieren:

</div>

 

<div>

\<pre\>

</div>

 

<div>

\<pre\>

</div>

−

<div>

sudo apt-get install dpkg-dev fakeroot debhelper ant m4

</div>

\+

<div>

sudo apt-get install dpkg-dev fakeroot debhelper ant m4
[default-jdk]{.underline}

</div>

 

<div>

\</pre\>

</div>

 

<div>

\</pre\>

</div>

 

 

−

<div>

~~Und dann~~ das Packet bauen:

</div>

\+

<div>

[Schlußendlich]{.underline} das Packet bauen[, welches ein Verzeichnis
höher abgelegt wird]{.underline}:

</div>

 

<div>

\<pre\>

</div>

 

<div>

\<pre\>

</div>

 

<div>

ant deb

</div>

 

<div>

ant deb

</div>

 

<div>

\</pre\>

</div>

 

<div>

\</pre\>

</div>
