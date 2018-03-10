Fr:DebianInstall
================

Date: 2014-05-28 18:21:55

[L\'installation de YaCy sur Debian ou Ubuntu: ]{.autocomment} Java 7

← Nächstältere Version

Version vom 28. Mai 2014, 16:21 Uhr

Zeile 18:

Zeile 18:

 

 

 

<div>

Si vous ne disposez pas déjà du JDK Java (installé), il se peut que vous
avez besoin d\'utiliser cette commande à la place (sur Ubuntu 10.04
\[Lucid\],  the \<tt\>yacy\</tt\> version du paquet ne tire pas dans
\<tt\>openjdk-6-jre\</tt\> appropriée en tant que dépendance) :

</div>

 

<div>

Si vous ne disposez pas déjà du JDK Java (installé), il se peut que vous
avez besoin d\'utiliser cette commande à la place (sur Ubuntu 10.04
\[Lucid\],  the \<tt\>yacy\</tt\> version du paquet ne tire pas dans
\<tt\>openjdk-6-jre\</tt\> appropriée en tant que dépendance) :

</div>

−

<div>

  apt-get install openjdk-~~6~~-jre-headless yacy

</div>

\+

<div>

  apt-get install openjdk-[7]{.underline}-jre-headless yacy

</div>

 

 

 

<div>

\'\'\'Attention ! YaCy 1.5 ne fonctionne pas avec openjdk-7-jre\'\'\'

</div>

 

<div>

\'\'\'Attention ! YaCy 1.5 ne fonctionne pas avec openjdk-7-jre\'\'\'

</div>
