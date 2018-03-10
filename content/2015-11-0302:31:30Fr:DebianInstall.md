Fr:DebianInstall
================

Date: 2015-11-03 02:31:30

[Modifier l\'emplacement des données /var/lib/yacy :: ]{.autocomment}

← Nächstältere Version

Version vom 3. November 2015, 01:31 Uhr

Zeile 60:

Zeile 60:

 

<div>

     mount \--bind /chemin\_de\_montage/yacy /var/lib/yacy

</div>

 

<div>

     mount \--bind /chemin\_de\_montage/yacy /var/lib/yacy

</div>

 

<div>

     /etc/init.d/yacy start

</div>

 

<div>

     /etc/init.d/yacy start

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Ou pour un montage automatique au démarrage éditer le fichier
\'\'\'/etc/fstab\'\'\' est rajouter la ligne :
\'\'\'/chemin\_de\_montage/yacy /var/lib/yacy none
bind\'\'\']{.underline}

</div>

 

 

 

<div>

== Gestion de YaCy ==

</div>

 

<div>

== Gestion de YaCy ==

</div>
