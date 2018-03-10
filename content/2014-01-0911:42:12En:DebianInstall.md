En:DebianInstall
================

Date: 2014-01-09 11:42:12

[Installation of YaCy on Debian: ]{.autocomment} headless sufficient

← Nächstältere Version

Version vom 9. Januar 2014, 10:42 Uhr

(Eine dazwischenliegende Version von einem Benutzer wird nicht
angezeigt)

Zeile 8:

Zeile 8:

 

<div>

  http://debian.yacy.net

</div>

 

<div>

  http://debian.yacy.net

</div>

 

 

−

<div>

~~Because direct editing of /etc/apt/sources.~~list ~~became depricated
create a new~~ file:

</div>

\+

<div>

[Create a debian source]{.underline} list file [for YaCy
sources]{.underline}:

</div>

−

<div>

~~touch /etc/apt/sources.list.d/yacy.list~~

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

~~And insert into this file the neccessary information~~

</div>

\+

<div>

</div>

 

<div>

  echo \'deb http://debian.yacy.net ./\' \>
/etc/apt/sources.list.d/yacy.list  

</div>

 

<div>

  echo \'deb http://debian.yacy.net ./\' \>
/etc/apt/sources.list.d/yacy.list  

</div>

 

 

Zeile 20:

Zeile 17:

 

<div>

And finally install YaCy itself

</div>

 

<div>

And finally install YaCy itself

</div>

 

<div>

  apt-get update

</div>

 

<div>

  apt-get update

</div>

−

<div>

  apt-get install openjdk-6-jre \# ~~just if openjdk-~~6~~-jre or
openjdk-6-jre-~~headless ~~isn\'t installed~~

</div>

\+

<div>

  apt-get install openjdk-6-jre[-headless]{.underline} \#
[java]{.underline} 6 [is sufficient, only a]{.underline} headless
[version is needed]{.underline}

</div>

 

<div>

  apt-get install yacy

</div>

 

<div>

  apt-get install yacy

</div>

 

 
