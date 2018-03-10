De:DebianInstall
================

Date: 2014-01-28 10:43:21

[YaCy unter Debian installieren: ]{.autocomment} ein bisschen kürzer

← Nächstältere Version

Version vom 28. Januar 2014, 09:43 Uhr

Zeile 6:

Zeile 6:

 

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
es einen Update-Server:

</div>

\+

<div>

Man kann die Packages über den apt-get install Prozess laden, dazu gibt
es einen Update-Server: [http://debian.yacy.net]{.underline}

</div>

 

 

−

<div>

~~http://debian.yacy.net~~

</div>

\+

<div>

[Als User root]{.underline} eine eigene [source-]{.underline}Datei für
YaCy erstellen:

</div>

−

<div>

 

</div>

\+

<div>

  echo \'deb http://debian.yacy.net ./\' [\>]{.underline}\>
/etc/apt/sources.list.d/yacy.list

</div>

−

<div>

~~weil das direkte Editieren von /etc/apt/sources.list deprecated
wurde~~ eine eigene Datei für YaCy erstellen:

</div>

\+

<div>

</div>

−

<div>

~~touch /etc/apt/sources.list.d/yacy.list~~

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

~~und dort hinein die Information über den Update-Server und das Package
schreiben~~

</div>

\+

<div>

</div>

−

<div>

  echo \'deb http://debian.yacy.net ./\' \>
/etc/apt/sources.list.d/yacy.list

</div>

\+

<div>

</div>

 

 

 

<div>

den Entwickler-Release-Key installieren über einen der beiden
Möglichkeiten:

</div>

 

<div>

den Entwickler-Release-Key installieren über einen der beiden
Möglichkeiten:

</div>
