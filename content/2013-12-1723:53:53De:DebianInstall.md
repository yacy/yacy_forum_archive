De:DebianInstall
================

Date: 2013-12-17 23:53:53

[Bei Debian ist das Editieren der sources.list in dem Zusammenhang
depricated geworden: ]{.autocomment}

← Nächstältere Version

Version vom 17. Dezember 2013, 22:53 Uhr

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

= YaCy unter Debian ~~bzw. Ubuntu~~ installieren =

</div>

\+

<div>

= YaCy unter Debian installieren =

</div>

 

 

−

<div>

Eine Anleitung zum ~~selberbauen~~ des ~~debianpakets~~
\[\[DebianPaketBauen\|hier\]\].

</div>

\+

<div>

Eine Anleitung zum [Selberbauen]{.underline} des
[Debianpaketes]{.underline} \[\[DebianPaketBauen\|hier\]\].

</div>

 

 

 

<div>

Man kann die Packages über den apt-get install Prozess laden, dazu gibt
es einen Update-Server:

</div>

 

<div>

Man kann die Packages über den apt-get install Prozess laden, dazu gibt
es einen Update-Server:

</div>

Zeile 10:

Zeile 10:

 

<div>

  http://debian.yacy.net

</div>

 

<div>

  http://debian.yacy.net

</div>

 

 

−

<div>

~~in~~ das /etc/apt/sources.list ~~muss eingetragen werden~~:

</div>

\+

<div>

[weil]{.underline} das [direkte Editieren von]{.underline}
/etc/apt/sources.list [deprecated wurde eine eigene Datei für YaCy
erstellen]{.underline}:

</div>

−

<div>

  ~~\# Mehr unter
http:~~//~~www~~.~~yacy-websuche~~.~~de~~/~~wiki/index~~.~~php/De:DebianInstall~~

</div>

\+

<div>

  [touch]{.underline}
/[etc]{.underline}/[apt/sources]{.underline}.[list]{.underline}.[d]{.underline}/[yacy]{.underline}.[list]{.underline}

</div>

−

<div>

  ~~\<nowiki\>~~deb http://debian.yacy.net ./~~\</nowiki~~\>

</div>

\+

<div>

 

</div>

 

\+

<div>

[und dort hinein die Information über den Update-Server und das Package
schreiben]{.underline}

</div>

 

\+

<div>

  [echo \']{.underline}deb http://debian.yacy.net ./[\']{.underline} \>
[/etc/apt/sources.list.d/yacy.list]{.underline}

</div>

 

 

 

<div>

den Entwickler-Release-Key installieren über einen der beiden
Möglichkeiten:

</div>

 

<div>

den Entwickler-Release-Key installieren über einen der beiden
Möglichkeiten:

</div>
