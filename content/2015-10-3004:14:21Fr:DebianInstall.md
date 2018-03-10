Fr:DebianInstall
================

Date: 2015-10-30 04:14:21

[Modifier l\'emplacement des données /var/lib/yacy :: ]{.autocomment}

← Nächstältere Version

Version vom 30. Oktober 2015, 03:14 Uhr

Zeile 53:

Zeile 53:

 

<div>

     /etc/init.d/yacy stop

</div>

 

<div>

     /etc/init.d/yacy stop

</div>

 

<div>

     mv /var/lib/yacy /chemin\_de\_montage/yacy

</div>

 

<div>

     mv /var/lib/yacy /chemin\_de\_montage/yacy

</div>

−

<div>

     chown yacy:yacy /chemin\_de\_montage/yacy

</div>

\+

<div>

     chown [-R]{.underline} yacy:yacy /chemin\_de\_montage/yacy

</div>

 

 

 

<div>

\#2 - Sous forme de script Bash pour démarrer Yacy, on monte le nouvel
emplacement contenant les données, vers l\'emplacement originel :

</div>

 

<div>

\#2 - Sous forme de script Bash pour démarrer Yacy, on monte le nouvel
emplacement contenant les données, vers l\'emplacement originel :

</div>
