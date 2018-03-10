En:GentooInstall
================

Date: 2014-11-20 13:34:07

[HowTo install YaCy on Gentoo: ]{.autocomment}

← Nächstältere Version

Version vom 20. November 2014, 12:34 Uhr

Zeile 4:

Zeile 4:

 

<div>

=HowTo install YaCy on Gentoo=

</div>

 

<div>

=HowTo install YaCy on Gentoo=

</div>

 

 

−

<div>

~~Here is the (very old) experimentall ebuild~~. ~~You have to rename it
like the current release-number~~.

</div>

\+

<div>

[Gentoo Bug for yacy:
https://bugs]{.underline}.[gentoo]{.underline}.[org/show\_bug.cgi?id=100108]{.underline}

</div>

 

 

−

<div>

~~i~~.~~E~~. ~~for
\<code\>yacy\_v0.61\_20081003\_5246.tar.gz\<~~/~~code\> rename it to:
\<code\>~~yacy~~-0.61.20081003.5246.ebuild\</code\>~~

</div>

\+

<div>

[Current available ebuilds from overlays:
http://gpo]{.underline}.[zugaina]{.underline}.[org]{.underline}/[Search?search=]{.underline}yacy

</div>

 

 

−

<div>

~~\<pre\>\# Copyright 1999-2009 Gentoo Foundation~~

</div>

\+

<div>

[For example]{.underline}

</div>

−

<div>

~~\# Distributed under the terms of the GNU General Public License v2~~

</div>

\+

<div>

</div>

 

 

−

<div>

~~inherit eutils versionator~~

</div>

\+

<div>

[\<code\>]{.underline}

</div>

−

<div>

 

</div>

\+

<div>

[layman]{.underline} -[a flow && emerge]{.underline}
net-[misc]{.underline}/yacy

</div>

−

<div>

~~MAJOR\_PV=\"\$(get\_version\_component\_range 1~~-~~2)\"~~

</div>

\+

<div>

\</[code]{.underline}\>

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

~~HOMEPAGE=\"http://www.yacy.~~net~~/\"~~

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

~~DEPEND=\"\>=virtual/jdk~~-~~1.5.0\"~~

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

~~S=\"\${WORKDIR}~~/yacy~~\"~~

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

~~}~~\</~~pre~~\>

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

~~There was special svn-ebuilds and initscripts, but there are no more
maintained. If you need some inspirations take a look at the archive
http://yacy.deruwe.de/old%20outdated%20stuff/~~

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

~~\* https://bugs.gentoo.org/show\_bug.cgi?id=100108~~

</div>

\+

<div>

</div>

 

 

 

<div>

\[\[Category:En:Installation\]\]

</div>

 

<div>

\[\[Category:En:Installation\]\]

</div>
