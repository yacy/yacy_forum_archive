De:IntegrationMSIE
==================

Date: 2013-11-27 00:04:51

← Nächstältere Version

Version vom 26. November 2013, 23:04 Uhr

Zeile 8:

Zeile 8:

 

<div>

   \<Url type=\"text/html\"  

</div>

 

<div>

   \<Url type=\"text/html\"  

</div>

 

<div>

       method=\"get\"

</div>

 

<div>

       method=\"get\"

</div>

−

<div>

      
template=\"http://localhost:~~8080~~/yacysearch.html?search={searchTerms}\"/\>

</div>

\+

<div>

      
template=\"http://localhost:[8090]{.underline}/yacysearch.html?search={searchTerms}\"/\>

</div>

 

<div>

\</OpenSearchDescription\>\</nowiki\>\</pre\>Die Adresse zum YaCy-Peer,
der für die Suche benutzt werden soll, muss angepasst werden, wenn Peer
und Browser nicht auf dem selben Rechner laufen.

</div>

 

<div>

\</OpenSearchDescription\>\</nowiki\>\</pre\>Die Adresse zum YaCy-Peer,
der für die Suche benutzt werden soll, muss angepasst werden, wenn Peer
und Browser nicht auf dem selben Rechner laufen.

</div>

 

<div>

\*Nun muss eine HTML-Seite erzeugt werden, die folgenden Inhalt
hat:\<pre\>\<nowiki\>\<html\>

</div>

 

<div>

\*Nun muss eine HTML-Seite erzeugt werden, die folgenden Inhalt
hat:\<pre\>\<nowiki\>\<html\>

</div>

Zeile 20:

Zeile 20:

 

 

 

<div>

===Hinweise===

</div>

 

<div>

===Hinweise===

</div>

−

<div>

\*Dem YaCy-Peer können noch weiter Parameter übergeben werden, die
verschiedene Eigenschaften der Suche bestimmen. Hierzu muss die Adresse
der Peers wie folgt erweitert werden:
\<pre\>\<nowiki\>http://localhost:~~8080~~/yacysearch.html?search={searchTerms}&amp;amp;parameter1=wert&amp;amp;parameter2=wert\</nowiki\>\</pre\>

</div>

\+

<div>

\*Dem YaCy-Peer können noch weiter Parameter übergeben werden, die
verschiedene Eigenschaften der Suche bestimmen. Hierzu muss die Adresse
der Peers wie folgt erweitert werden:
\<pre\>\<nowiki\>http://localhost:[8090]{.underline}/yacysearch.html?search={searchTerms}&amp;amp;parameter1=wert&amp;amp;parameter2=wert\</nowiki\>\</pre\>

</div>

 

<div>

\*Die oben angegebene XML-Datei ist lediglich ein sehr einfaches
Beispiel. Nähere Informationen sind auf den folgenden Seiten zu finden.

</div>

 

<div>

\*Die oben angegebene XML-Datei ist lediglich ein sehr einfaches
Beispiel. Nähere Informationen sind auf den folgenden Seiten zu finden.

</div>

 

<div>

\*\*\[http://www.microsoft.com/windows/ie/searchguide/default\_new.mspx\|Add
Search Providers to Internet Explorer 7\]

</div>

 

<div>

\*\*\[http://www.microsoft.com/windows/ie/searchguide/default\_new.mspx\|Add
Search Providers to Internet Explorer 7\]

</div>
