De:WWWIntegration
=================

Date: 2013-03-11 11:05:10

port fix

← Nächstältere Version

Version vom 11. März 2013, 10:05 Uhr

Zeile 5:

Zeile 5:

 

<div>

Das Live-Search Eingabefeld reagiert sofort mit bei der Eingabe und
lässt ein Pop-Fenster mit Suchergebnissen erscheinen. Es lässt sich ganz
leicht auf deine Webseite integrieren, nutze dazu einfach das folgende
Java-Script Snippet:

</div>

 

<div>

Das Live-Search Eingabefeld reagiert sofort mit bei der Eingabe und
lässt ein Pop-Fenster mit Suchergebnissen erscheinen. Es lässt sich ganz
leicht auf deine Webseite integrieren, nutze dazu einfach das folgende
Java-Script Snippet:

</div>

 

<div>

\<pre\>

</div>

 

<div>

\<pre\>

</div>

−

<div>

   \<script src=\"http://\<deine Peer
IP\>:~~8080~~/yacy/ui/js/jquery-1.3.2.min.js\" 
type=\"text/javascript\"\>\</script\>

</div>

\+

<div>

   \<script src=\"http://\<deine Peer
IP\>:[8090]{.underline}/yacy/ui/js/jquery-1.3.2.min.js\" 
type=\"text/javascript\"\>\</script\>

</div>

 

<div>

   \<script\>       

</div>

 

<div>

   \<script\>       

</div>

 

<div>

   \$(document).ready(function() {

</div>

 

<div>

   \$(document).ready(function() {

</div>

 

<div>

       yconf = {

</div>

 

<div>

       yconf = {

</div>

−

<div>

       url    : \<deine Peer IP\>:~~8080~~,

</div>

\+

<div>

       url    : \<deine Peer IP\>:[8090]{.underline},

</div>

 

<div>

       logo  : \'/yacy/ui/img/yacy-logo.png\',

</div>

 

<div>

       logo  : \'/yacy/ui/img/yacy-logo.png\',

</div>

 

<div>

       link  : \'http://www.yacy.net\',

</div>

 

<div>

       link  : \'http://www.yacy.net\',

</div>

Zeile 23:

Zeile 23:

 

<div>

   \</script\>

</div>

 

<div>

   \</script\>

</div>

 

<div>

   \<div id=\"yacylivesearch\"\>

</div>

 

<div>

   \<div id=\"yacylivesearch\"\>

</div>

−

<div>

     \<form id=\"ysearch\" method=\"get\" accept-charset=\"UTF-8\"
action=\"http://139.30.18.9:~~8080~~/yacysearch.html\"\>

</div>

\+

<div>

     \<form id=\"ysearch\" method=\"get\" accept-charset=\"UTF-8\"
action=\"http://139.30.18.9:[8090]{.underline}/yacysearch.html\"\>

</div>

 

<div>

     Live Search \<input name=\"query\" id=\"yquery\" class=\"fancy\"
type=\"text\" size=\"15\" maxlength=\"80\" value=\"\"/\>

</div>

 

<div>

     Live Search \<input name=\"query\" id=\"yquery\" class=\"fancy\"
type=\"text\" size=\"15\" maxlength=\"80\" value=\"\"/\>

</div>

 

<div>

     \<input type=\"hidden\" name=\"verify\" value=\"false\" /\>

</div>

 

<div>

     \<input type=\"hidden\" name=\"verify\" value=\"false\" /\>

</div>

Zeile 211:

Zeile 211:

 

 

 

<div>

==Mediawiki==

</div>

 

<div>

==Mediawiki==

</div>

−

<div>

http://localhost:~~8080~~/ConfigWikiSearch.html

</div>

\+

<div>

http://localhost:[8090]{.underline}/ConfigWikiSearch.html

</div>

 

 

 

<div>

==phpBB==

</div>

 

<div>

==phpBB==

</div>

−

<div>

http://localhost:~~8080~~/ConfigPHPBB3Search.html

</div>

\+

<div>

http://localhost:[8090]{.underline}/ConfigPHPBB3Search.html

</div>
