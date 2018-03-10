De:GentooInstall
================

Date: 2014-11-20 13:36:17

[YaCy unter Gentoo installieren: ]{.autocomment}

← Nächstältere Version

Version vom 20. November 2014, 12:36 Uhr

Zeile 5:

Zeile 5:

 

<div>

YaCy kann auch unter Gentoo \"manuell\" installiert werden, mehr dazu
siehe \[\[De:GenericInstall\]\].

</div>

 

<div>

YaCy kann auch unter Gentoo \"manuell\" installiert werden, mehr dazu
siehe \[\[De:GenericInstall\]\].

</div>

 

 

−

<div>

Es ~~gibt aber~~ auch ein ~~experimentelles Ebuild~~. ~~Dieses muss
entsprechend der Versionsnummer des aktuellen Release-Archives benannt
werden~~. ~~Es installiert~~/~~updatet nur die Programmdateien von YaCy,
nicht das Datenverzeichnis oder getroffene Einstellungen. Diese bleiben
auch bei der Deinstallation über das Ebuild erhalten und müssen bei
Bedarf manuell gelöscht werden.~~

</div>

\+

<div>

Es [existieren]{.underline} auch ein [paar aktuelle ebuilds in
verschieden overlays:
http://gpo]{.underline}.[zugaina]{.underline}.[org]{.underline}/[Search?search=yacy]{.underline}

</div>

 

 

−

<div>

z.~~B.: für die Version
\<code\>yacy\_v0.61\_20081003\_5246.tar.gz\</code\> muß das Ebuild
heißen: \<code\>yacy-0.61.20081003.5246~~.~~ebuild\</code\>~~

</div>

\+

<div>

[Damit kann yacy]{.underline} z.[b]{.underline}. [mittels]{.underline}

</div>

 

 

−

<div>

\<~~pre~~\>~~\# Copyright 1999~~-~~2009 Gentoo Foundation~~

</div>

\+

<div>

\<[code]{.underline}\>

</div>

−

<div>

~~\# Distributed under the terms of the GNU General Public License v2~~

</div>

\+

<div>

[layman]{.underline} -[a flow && emerge net-misc/yacy]{.underline}

</div>

 

\+

<div>

[\</code\>]{.underline}

</div>

 

 

−

<div>

~~inherit eutils versionator~~

</div>

\+

<div>

[installiert werden]{.underline}.

</div>

−

<div>

 

</div>

\+

<div>

</div>

−

<div>

~~MAJOR\_PV=\"\$(get\_version\_component\_range 1-2)\"~~

</div>

\+

<div>

</div>

−

<div>

~~REL\_PV=\"\$(get\_version\_component\_range 3)\"~~

</div>

\+

<div>

</div>

−

<div>

~~SVN\_PV=\"\$(get\_version\_component\_range 4)\"~~

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

~~DESCRIPTION=\"p2p based distributed web-search engine - latest stable
binary\"~~

</div>

\+

<div>

</div>

−

<div>

~~HOMEPAGE=\"http://www.yacy.net/\"~~

</div>

\+

<div>

</div>

−

<div>

~~SRC\_URI=\"http://www.yacy.net/release/yacy\_v\${MAJOR\_PV}\_\${REL\_PV}\_\${SVN\_PV}.tar.gz\"~~

</div>

\+

<div>

</div>

−

<div>

~~SLOT=\"0\"~~

</div>

\+

<div>

</div>

−

<div>

~~KEYWORDS=\"\~x86 \~amd64\"~~

</div>

\+

<div>

</div>

−

<div>

~~DEPEND=\"\>=virtual/jdk-1.5.0\"~~

</div>

\+

<div>

</div>

−

<div>

~~LICENSE=\"GPL-2\"~~

</div>

\+

<div>

</div>

−

<div>

~~IUSE=\"\"~~

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

~~S=\"\${WORKDIR}/yacy\"~~

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

~~src\_install() {~~

</div>

\+

<div>

</div>

−

<div>

~~dodir /opt~~

</div>

\+

<div>

</div>

−

<div>

~~mv \"\${S}\" \"\${D}/opt/\${PN}\"~~

</div>

\+

<div>

</div>

−

<div>

~~chown -R \${PN}:\${PN} \"\${D}/opt/\${PN}\"~~

</div>

\+

<div>

</div>

−

<div>

~~}~~

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

~~pkg\_setup() {~~

</div>

\+

<div>

</div>

−

<div>

~~enewgroup \${PN}~~

</div>

\+

<div>

</div>

−

<div>

~~enewuser \${PN} -1 /bin/bash /opt/\${PN} \${PN}~~

</div>

\+

<div>

</div>

−

<div>

~~}~~

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

~~pkg\_postinst() {~~

</div>

\+

<div>

</div>

−

<div>

~~einfo \"This is the plain install without initscripts.\"~~

</div>

\+

<div>

</div>

−

<div>

~~einfo \"Keep in mind, YaCy works in /opt/yacy/DATA\"~~

</div>

\+

<div>

</div>

−

<div>

~~einfo \"so its a good idea to move it to /var und symlink it.\"~~

</div>

\+

<div>

</div>

−

<div>

~~einfo \"Logfiles are in /opt/yacy/DATA/LOG instead of /var/log\"~~

</div>

\+

<div>

</div>

−

<div>

~~einfo \"For details (in german) about YaCy on Gentoo look at:\"~~

</div>

\+

<div>

</div>

−

<div>

~~einfo \" http://yacy-websuche.de/wiki/index.php/De:GentooInstall\"~~

</div>

\+

<div>

</div>

−

<div>

~~}\</pre\>~~

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

~~Spezielle SVN-Ebuilds / Initscripte gab es einmal. Deren Entwirklung
wurde jedoch eingestellt. Wer sich Inspirationen holen möchte dem sei
das Archiv der alten Ebuild und Scripte unter
http://yacy.deruwe.de/old%20outdated%20stuff/ empfohlen~~.

</div>

\+

<div>

</div>

 

 

 

<div>

\* https://bugs.gentoo.org/show\_bug.cgi?id=100108

</div>

 

<div>

\* https://bugs.gentoo.org/show\_bug.cgi?id=100108

</div>
