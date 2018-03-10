Fr:DebianInstall
================

Date: 2016-03-02 18:24:53

Corrections orthographe et syntaxe, liens interwiki mis en bas

← Nächstältere Version

Version vom 2. März 2016, 17:24 Uhr

Zeile 1:

Zeile 1:

−

<div>

~~{{interwikiEN\|En:DebianInstall}}~~

</div>

\+

<div>

= [Installer]{.underline} YaCy sur Debian ou Ubuntu =

</div>

−

<div>

~~{{interwikiDE\|De:DebianInstall}}~~

</div>

\+

<div>

</div>

−

<div>

~~{{interwikiES\|Es:Instalación en Debian}}~~

</div>

\+

<div>

</div>

−

<div>

~~{{interwikiFR\|Fr:DebianInstall}}~~

</div>

\+

<div>

</div>

−

<div>

~~{{interwikiRU\|Ru:Debian Установка}}~~

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

= ~~L\'installation de~~ YaCy sur Debian ou Ubuntu =

</div>

\+

<div>

</div>

 

 

−

<div>

~~Installation~~ sur les systèmes d\'exploitation GNU/Linux ~~basée~~
sur Debian est facile en utilisant ~~notre~~ dépôt Debian :

</div>

\+

<div>

[L\'installation]{.underline} sur les systèmes d\'exploitation GNU/Linux
[basés]{.underline} sur Debian est facile en utilisant [le]{.underline}
dépôt Debian [YaCy]{.underline} :

</div>

 

 

 

<div>

  http://debian.yacy.net

</div>

 

<div>

  http://debian.yacy.net

</div>

 

 

−

<div>

Pour utiliser ce serveur, ~~copiez ceci~~ à votre fichier
\'\'\'/etc/apt/sources.list\'\'\' :

</div>

\+

<div>

Pour utiliser ce serveur, [ajoutez]{.underline} à votre fichier
\'\'\'/etc/apt/sources.list\'\'\' :

</div>

 

<div>

  \<nowiki\>deb http://debian.yacy.net ./\</nowiki\>

</div>

 

<div>

  \<nowiki\>deb http://debian.yacy.net ./\</nowiki\>

</div>

 

 

Zeile 18:

Zeile 12:

 

<div>

  \<nowiki\>gpg -a \--export 1F968B3903D886E7 \| sudo apt-key add
-\</nowiki\>

</div>

 

<div>

  \<nowiki\>gpg -a \--export 1F968B3903D886E7 \| sudo apt-key add
-\</nowiki\>

</div>

 

 

−

<div>

Ensuite, vous pouvez installer YaCy avec les commandes suivantes.
~~S\'il vous plaît~~ noter que le dépôt n\'a pas de clés GPG ~~mis en
place à partir de Mars~~ 2013, vous verrez généralement un message
d\'avertissement ~~concernant~~ ce lors de l\'installation.

</div>

\+

<div>

Ensuite, vous pouvez installer YaCy avec les commandes suivantes.
[Veuillez]{.underline} noter que le dépôt n\'a pas de clés GPG [depuis
mars]{.underline} 2013, [donc]{.underline} vous verrez généralement un
message d\'avertissement [à]{.underline} ce [propos]{.underline} lors de
l\'installation.

</div>

 

 

 

<div>

  apt-get update

</div>

 

<div>

  apt-get update

</div>

 

<div>

  apt-get install yacy

</div>

 

<div>

  apt-get install yacy

</div>

 

 

−

<div>

Si vous ne disposez pas déjà du JDK Java ~~(~~installé~~)~~, il se peut
que vous ~~avez~~ besoin d\'utiliser cette commande à la place (sur
Ubuntu 10.04 \[Lucid\], ~~the~~ \<tt\>yacy\</tt\> ~~version du paquet~~
ne tire pas ~~dans~~ \<tt\>openjdk-6-jre\</tt\> ~~appropriée en tant que
dépendance~~) :

</div>

\+

<div>

Si vous ne disposez pas déjà du JDK Java installé, il se peut que vous
[ayez]{.underline} besoin d\'utiliser cette commande à la place ([par
exemple,]{.underline} sur Ubuntu 10.04 \[Lucid\], [la version du
paquet]{.underline} \<tt\>yacy\</tt\> ne tire pas [la dépendance
appropriée]{.underline} \<tt\>openjdk-6-jre\</tt\>) :

</div>

 

<div>

  apt-get install openjdk-7-jre-headless yacy

</div>

 

<div>

  apt-get install openjdk-7-jre-headless yacy

</div>

 

 

Zeile 32:

Zeile 26:

 

<div>

  /usr/share/yacy

</div>

 

<div>

  /usr/share/yacy

</div>

 

 

−

<div>

Les ~~Données~~ (voir plus bas pour modifier l\'emplacement des données,
si la DHT a été désactivée par manque ~~que de mémoire~~) :

</div>

\+

<div>

Les [données]{.underline} (voir plus bas pour modifier l\'emplacement
des données, si la DHT a été désactivée par manque [d\'espace
disponible]{.underline}) :

</div>

 

 

 

<div>

  /var/lib/yacy

</div>

 

<div>

  /var/lib/yacy

</div>

Zeile 50:

Zeile 44:

 

<div>

==== Modifier l\'emplacement des données /var/lib/yacy : ====  

</div>

 

<div>

==== Modifier l\'emplacement des données /var/lib/yacy : ====  

</div>

 

 

−

<div>

\#1 - On ~~commencer~~ par déplacer les données vers ~~leurs nouvelles
emplacements~~.\<br /\>

</div>

\+

<div>

\#1 - On [commence]{.underline} par déplacer les données vers [leur
nouvel emplacement]{.underline}.\<br /\>

</div>

 

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

Zeile 61:

Zeile 55:

 

<div>

     /etc/init.d/yacy start

</div>

 

<div>

     /etc/init.d/yacy start

</div>

 

 

−

<div>

Ou pour un montage automatique au démarrage éditer le fichier
\'\'\'/etc/fstab\'\'\' ~~est~~ rajouter la ligne :
\'\'\'/chemin\_de\_montage/yacy /var/lib/yacy none bind\'\'\'

</div>

\+

<div>

Ou pour un montage automatique au démarrage[,]{.underline} éditer le
fichier \'\'\'/etc/fstab\'\'\' [et]{.underline} rajouter la ligne :
\'\'\'/chemin\_de\_montage/yacy /var/lib/yacy none bind\'\'\'

</div>

 

 

 

<div>

== Gestion de YaCy ==

</div>

 

<div>

== Gestion de YaCy ==

</div>

−

<div>

Lorsque vous avez installé YaCy en utilisant le dépôt Debian, YaCy est
lancé automatiquement après ~~un~~ démarrage ~~OS~~, et s\'arrêta lors
de l\'arrêt.

</div>

\+

<div>

Lorsque vous avez installé YaCy en utilisant le dépôt Debian, YaCy est
lancé automatiquement après [le]{.underline} démarrage [du
système]{.underline}, et s\'arrêta lors de l\'arrêt.

</div>

 

 

−

<div>

Vous pouvez également démarrer et arrêter YaCy ~~à partir de la ligne de
commande~~ avec (~~doit être exécuté~~ en tant que root) :

</div>

\+

<div>

Vous pouvez également démarrer et arrêter YaCy
[manuellement]{.underline} avec [les commandes suivantes]{.underline}
([à exécuter]{.underline} en tant que root) :

</div>

 

 

 

<div>

  /etc/init.d/yacy start

</div>

 

<div>

  /etc/init.d/yacy start

</div>

Zeile 76:

Zeile 70:

 

<div>

  http://localhost:8090/

</div>

 

<div>

  http://localhost:8090/

</div>

 

 

−

<div>

~~mais vous~~ pouvez également définir un autre port pour
l\'~~interface~~ à l\'aide des pages d\'administration de YaCy.

</div>

\+

<div>

[Vous]{.underline} pouvez également définir un autre port pour
l\'[interfe web]{.underline} à l\'aide des pages d\'administration de
YaCy.

</div>

 

<div>

Un port 80 est possible, mais il est préférable d\'obtenir l\'accès à ce
port en utilisant un \[\[Fr:Portforwarding \| Portforwarding\]\].

</div>

 

<div>

Un port 80 est possible, mais il est préférable d\'obtenir l\'accès à ce
port en utilisant un \[\[Fr:Portforwarding \| Portforwarding\]\].

</div>

 

 

 

<div>

== Mises à jour automatiques ==

</div>

 

<div>

== Mises à jour automatiques ==

</div>

−

<div>

~~Lorsqu\'il~~ est ~~configuré de cette façon~~, ~~le YaCy-interne~~
mise à jour automatique ne fonctionne pas. Une mise à jour automatique
doit être faite avec les outils ~~OS. dire~~ avec une commande crontab.
Un exemple ~~en~~ est la ligne suivante, que vous devez écrire dans
\'\'\'/etc/crontab\'\'\'

</div>

\+

<div>

[Lorsque YaCy]{.underline} est [installé en tant que paquet
Debian]{.underline}, [la]{.underline} mise à jour automatique
[interne]{.underline} ne fonctionne pas. Une mise à jour automatique
doit être faite avec les outils [système, par exemple]{.underline} avec
une commande crontab. Un exemple est [fourni à]{.underline} la ligne
suivante, que vous devez écrire dans \'\'\'/etc/crontab\'\'\'

</div>

 

 

 

<div>

  0 6 \* \* \* root apt-get update && apt-get -y \--force-yes install
yacy

</div>

 

<div>

  0 6 \* \* \* root apt-get update && apt-get -y \--force-yes install
yacy

</div>

 

 

−

<div>

Pour Ubuntu, la ligne ci-dessus n\'est valable que pour le fichier
crontab système (située dans /etc/crontab) - vous pouvez éditer ce
fichier sur plus ~~récente~~ Ubuntu ~~OS~~ directement sans utiliser la
commande crontab. Voici les commentaires du fichier dans Ubuntu 12.04 :

</div>

\+

<div>

Pour Ubuntu, la ligne ci-dessus n\'est valable que pour le fichier
crontab système (située dans /etc/crontab) - vous pouvez éditer ce
fichier sur [les versions]{.underline} plus [récentes
d\']{.underline}Ubuntu directement sans utiliser la commande crontab.
Voici les commentaires du fichier dans Ubuntu 12.04 :

</div>

 

 

 

<div>

  \# /etc/crontab: system-wide crontab

</div>

 

<div>

  \# /etc/crontab: system-wide crontab

</div>

Zeile 107:

Zeile 101:

 

<div>

  0 6 \* \* \* /usr/bin/apt-get update && /usr/bin/apt-get -y
\--force-yes install yacy

</div>

 

<div>

  0 6 \* \* \* /usr/bin/apt-get update && /usr/bin/apt-get -y
\--force-yes install yacy

</div>

 

 

−

<div>

Veuillez noter qu\'il n\'ya pas de nom d\'utilisateur sur la ligne
ci-dessus, et les chemins absolus ~~(plein)~~ sont utilisés ici pour
éviter les problèmes de localisation binaires!

</div>

\+

<div>

Veuillez noter qu\'il n\'ya pas de nom d\'utilisateur sur la ligne
ci-dessus, et les chemins absolus sont utilisés ici pour éviter les
problèmes de localisation [des]{.underline} binaires!

</div>

 

 

 

<div>

== Étapes suivantes ==

</div>

 

<div>

== Étapes suivantes ==

</div>

−

<div>

Après avoir configuré YaCy, vous pouvez également définir une
\[\[Fr:StaticIP \| IP Statique\]\] pour ~~obtenir~~ une adresse IP
unique à votre pairs YaCy.

</div>

\+

<div>

Après avoir configuré YaCy, vous pouvez également définir une
\[\[Fr:StaticIP \| IP Statique\]\] pour [assigner]{.underline} une
adresse IP unique à votre pairs YaCy.

</div>

 

 

 

<div>

\[\[Kategorie: Fr:HOWTO\]\]

</div>

 

<div>

\[\[Kategorie: Fr:HOWTO\]\]

</div>

Zeile 117:

Zeile 111:

 

<div>

\[\[Kategorie: Linux\]\]

</div>

 

<div>

\[\[Kategorie: Linux\]\]

</div>

 

 

−

<div>

~~{{interwikiDE\|De:DebianInstall}}~~

</div>

 

−

<div>

~~{{interwikiES\|Es:Instalación en Debian}}~~

</div>

 

 

<div>

{{interwikiEN\|En:DebianInstall}}

</div>

 

<div>

{{interwikiEN\|En:DebianInstall}}

</div>

 

\+

<div>

[{{interwikiDE\|De:DebianInstall}}]{.underline}

</div>

 

\+

<div>

[{{interwikiRU\|Ru:Debian Установка}}]{.underline}

</div>
