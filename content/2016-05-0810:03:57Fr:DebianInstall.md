Fr:DebianInstall
================

Date: 2016-05-08 10:03:57

[Gestion de YaCy: ]{.autocomment} Ajout systemctl pour gérer le
lancement automatique

← Nächstältere Version

Version vom 8. Mai 2016, 08:03 Uhr

Zeile 65:

Zeile 65:

 

<div>

  /etc/init.d/yacy restart

</div>

 

<div>

  /etc/init.d/yacy restart

</div>

 

<div>

  /etc/init.d/yacy stop

</div>

 

<div>

  /etc/init.d/yacy stop

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Vous pouvez aussi activer ou désactiver le lancement automatique au
démarrage en utilisant systemctl (en tant que root) :]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Activation du lancement automatique :]{.underline}

</div>

 

\+

<div>

[systemctl enable yacy]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Désactivation du lancement automatique :]{.underline}

</div>

 

\+

<div>

[systemctl disable yacy]{.underline}

</div>

 

 

 

<div>

Le serveur web de YaCy s\'exécute sur le port 8090 par défaut. Les pages
d\'administration sont à l\'adresse :

</div>

 

<div>

Le serveur web de YaCy s\'exécute sur le port 8090 par défaut. Les pages
d\'administration sont à l\'adresse :

</div>
