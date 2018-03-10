Fr:DebianInstall
================

Date: 2014-05-25 09:54:03

[L\'installation de YaCy sur Debian ou Ubuntu: ]{.autocomment}

← Nächstältere Version

Version vom 25. Mai 2014, 07:54 Uhr

Zeile 7:

Zeile 7:

 

<div>

Pour utiliser ce serveur, copiez ceci à votre fichier
\'\'\'/etc/apt/sources.list\'\'\' :

</div>

 

<div>

Pour utiliser ce serveur, copiez ceci à votre fichier
\'\'\'/etc/apt/sources.list\'\'\' :

</div>

 

<div>

  \<nowiki\>deb http://debian.yacy.net ./\</nowiki\>

</div>

 

<div>

  \<nowiki\>deb http://debian.yacy.net ./\</nowiki\>

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Pour vérifier la signature des paquets il faut ajouter une clé à votre
trousseau :]{.underline}

</div>

 

\+

<div>

[\<nowiki\>gpg \--keyserver pgpkeys.mit.edu \--recv-key
1F968B3903D886E7\</nowiki\>]{.underline}

</div>

 

\+

<div>

[\<nowiki\>gpg -a \--export 1F968B3903D886E7 \| sudo apt-key add
-\</nowiki\>]{.underline}

</div>

 

 

 

<div>

Ensuite, vous pouvez installer YaCy avec les commandes suivantes. S\'il
vous plaît noter que le dépôt n\'a pas de clés GPG mis en place à partir
de Mars 2013, vous verrez généralement un message d\'avertissement
concernant ce lors de l\'installation.

</div>

 

<div>

Ensuite, vous pouvez installer YaCy avec les commandes suivantes. S\'il
vous plaît noter que le dépôt n\'a pas de clés GPG mis en place à partir
de Mars 2013, vous verrez généralement un message d\'avertissement
concernant ce lors de l\'installation.

</div>
