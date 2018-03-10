De:IntegrationMSIE
==================

Date: 2014-10-23 01:17:15

← Nächstältere Version

Version vom 22. Oktober 2014, 23:17 Uhr

Zeile 2:

Zeile 2:

 

<div>

Der MS Internet Explorer bietet ab Version 7 die Möglichkeit,
Suchmaschinen einzubinden. Dazu geht man folgendermaßen vor:

</div>

 

<div>

Der MS Internet Explorer bietet ab Version 7 die Möglichkeit,
Suchmaschinen einzubinden. Dazu geht man folgendermaßen vor:

</div>

 

 

−

<div>

\*Zunächst muss eine kleine XML-Datei erzeugt und unter z.B. dem Namen
\'\'\'addyacy.xml\'\'\' abgespeichert werden.\<pre\>\<nowiki\>\<?xml
version=\"1.0\" encoding=\"UTF-8\"?\>

</div>

\+

<div>

\*Zunächst muss eine kleine XML-Datei erzeugt und unter z.B. dem Namen
\'\'\'addyacy.xml\'\'\' abgespeichert werden.

</div>

−

<div>

\<OpenSearchDescription xmlns=\"http://a9.com/-/spec/opensearch/1.1/\"\>

</div>

\+

<div>

 

</div>

−

<div>

~~ ~~ \<ShortName\>YaCy P2P Web Search Engine\</ShortName\>

</div>

\+

<div>

\<pre\>\<nowiki\>\<?xml version=\"1.0\" encoding=\"UTF-8\"?\>

</div>

−

<div>

~~ ~~ \<Description\>YaCy is a GPL\'ed open source P2P web search
engine.\</Description\>

</div>

\+

<div>

[]{.underline} \<OpenSearchDescription
xmlns=\"http://a9.com/-/spec/opensearch/1.1/\"\>

</div>

−

<div>

~~ ~~ \<Url type=\"text/html\"  

</div>

\+

<div>

[ ]{.underline} \<ShortName\>YaCy P2P Web Search Engine\</ShortName\>

</div>

−

<div>

~~     ~~ method=\"get\"

</div>

\+

<div>

[ ]{.underline} \<Description\>YaCy is a GPL\'ed open source P2P web
search engine.\</Description\>

</div>

−

<div>

~~     ~~
template=\"http://localhost:8090/yacysearch.html?search={searchTerms}\"/\>

</div>

\+

<div>

[ ]{.underline} \<Url type=\"text/html\"  

</div>

−

<div>

\</OpenSearchDescription\>\</nowiki\>\</pre\>Die Adresse zum YaCy-Peer,
der für die Suche benutzt werden soll, muss angepasst werden, wenn Peer
und Browser nicht auf dem selben Rechner laufen.

</div>

\+

<div>

[       ]{.underline} method=\"get\"

</div>

−

<div>

\*Nun muss eine HTML-Seite erzeugt werden, die folgenden Inhalt
hat:\<pre\>\<nowiki\>\<html\>

</div>

\+

<div>

[       ]{.underline}
template=\"http://localhost:8090/yacysearch.html?search={searchTerms}\"/\>

</div>

 

\+

<div>

\</OpenSearchDescription\>\</nowiki\>\</pre\>

</div>

 

\+

<div>

 

</div>

 

\+

<div>

Die Adresse zum YaCy-Peer, der für die Suche benutzt werden soll, muss
angepasst werden, wenn Peer und Browser nicht auf dem selben Rechner
laufen.

</div>

 

\+

<div>

\*Nun muss eine HTML-Seite erzeugt werden, die folgenden Inhalt hat:

</div>

 

\+

<div>

\<pre\>\<nowiki\>\<html\>

</div>

 

<div>

\<body\>

</div>

 

<div>

\<body\>

</div>

 

<div>

\<a href=\"\#\"
onClick=\"window.external.AddSearchProvider(&amp;quot;http://www.server.com/addyacy.xml&amp;quot;);\"\>YACY\</a\>

</div>

 

<div>

\<a href=\"\#\"
onClick=\"window.external.AddSearchProvider(&amp;quot;http://www.server.com/addyacy.xml&amp;quot;);\"\>YACY\</a\>

</div>
