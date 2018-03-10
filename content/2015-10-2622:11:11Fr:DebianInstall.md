Fr:DebianInstall
================

Date: 2015-10-26 22:11:11

[Emplacements des fichiers importants: ]{.autocomment}

← Nächstältere Version

Version vom 26. Oktober 2015, 21:11 Uhr

Zeile 52:

Zeile 52:

 

<div>

\#1 - On commencer par déplacer les données vers leurs nouvelles
emplacements.\<br /\>

</div>

 

<div>

\#1 - On commencer par déplacer les données vers leurs nouvelles
emplacements.\<br /\>

</div>

 

<div>

     /etc/init.d/yacy stop

</div>

 

<div>

     /etc/init.d/yacy stop

</div>

−

<div>

     mv /var/lib/yacy /~~chemin\_de\_montagne~~/yacy

</div>

\+

<div>

     mv /var/lib/yacy /[chemin\_de\_montage]{.underline}/yacy

</div>

−

<div>

     chown yacy:yacy /~~chemin\_de\_montagne~~/yacy

</div>

\+

<div>

     chown yacy:yacy /[chemin\_de\_montage]{.underline}/yacy

</div>

 

 

 

<div>

\#2 - Sous forme de script Bash pour démarrer Yacy, on monte le nouvel
emplacement contenant les données, vers l\'emplacement originel :

</div>

 

<div>

\#2 - Sous forme de script Bash pour démarrer Yacy, on monte le nouvel
emplacement contenant les données, vers l\'emplacement originel :

</div>

 

<div>

     \#!/bin/bash

</div>

 

<div>

     \#!/bin/bash

</div>

 

<div>

     /etc/init.d/yacy stop

</div>

 

<div>

     /etc/init.d/yacy stop

</div>

−

<div>

     mount \--bind /~~chemin\_de\_montagne~~/yacy /var/lib/yacy

</div>

\+

<div>

     mount \--bind /[chemin\_de\_montage]{.underline}/yacy /var/lib/yacy

</div>

 

<div>

     /etc/init.d/yacy start

</div>

 

<div>

     /etc/init.d/yacy start

</div>

 

 
