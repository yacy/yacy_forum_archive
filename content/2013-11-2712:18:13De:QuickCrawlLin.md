De:QuickCrawlLink
=================

Date: 2013-11-27 12:18:13

port 8090 fix

← Nächstältere Version

Version vom 27. November 2013, 11:18 Uhr

Zeile 2:

Zeile 2:

 

<div>

\[\[Bild:QuickCrawlLink.png\|left\|thumb\|Quick Crawl Link\]\]

</div>

 

<div>

\[\[Bild:QuickCrawlLink.png\|left\|thumb\|Quick Crawl Link\]\]

</div>

 

 

−

<div>

Durch Aufrufen des Link http://localhost:~~8080~~/QuickCrawlLink\_p.html
(bei YaCy auf \"\<code\>localhost\</code\>\", Port ~~8080~~) wird eine
Seite mit einem Link angezeigt, den man sich in die Lesenzeichenleiste
bzw. Favoritenleiste (Internet Explorer) ziehen kann.

</div>

\+

<div>

Durch Aufrufen des Link
http://localhost:[8090]{.underline}/QuickCrawlLink\_p.html (bei YaCy auf
\"\<code\>localhost\</code\>\", Port [8090]{.underline}) wird eine Seite
mit einem Link angezeigt, den man sich in die Lesenzeichenleiste bzw.
Favoritenleiste (Internet Explorer) ziehen kann.

</div>

 

 

 

<div>

Es wird damit eine Javascript-Funktion verlinkt, mit der man die gerade
im Browser angezeigte Seite automatisch in die Crawling-Queue des
YaCy-Peers setzen kann.

</div>

 

<div>

Es wird damit eine Javascript-Funktion verlinkt, mit der man die gerade
im Browser angezeigte Seite automatisch in die Crawling-Queue des
YaCy-Peers setzen kann.

</div>

 

 

−

<div>

Ist der YaCy-Peer nicht auf \"\<code\>localhost\</code\>\" erreichbar,
so kann statt \"\<code\>localhost:~~8080~~\</code\>\" die Syntax
\"\[Username\]:\[Passwort\]@\[YaCyIP\]:\[Port\]\" verwendet werden.

</div>

\+

<div>

Ist der YaCy-Peer nicht auf \"\<code\>localhost\</code\>\" erreichbar,
so kann statt \"\<code\>localhost:[8090]{.underline}\</code\>\" die
Syntax \"\[Username\]:\[Passwort\]@\[YaCyIP\]:\[Port\]\" verwendet
werden.

</div>

 

 

 

<div>

Alternativ zum Bookmarken des angezeigten Links kann auch direkt eine
Verknüpfung eingetragen werden:

</div>

 

<div>

Alternativ zum Bookmarken des angezeigten Links kann auch direkt eine
Verknüpfung eingetragen werden:

</div>

 

 

−

<div>

  \<pre\>javascript:w =
window.open(\'http://localhost:~~8080~~/QuickCrawlLink\_p.html?localIndexing=on&crawlingQ=on&xdstopw=on&title=\'
+

</div>

\+

<div>

  \<pre\>javascript:w =
window.open(\'http://localhost:[8090]{.underline}/QuickCrawlLink\_p.html?localIndexing=on&crawlingQ=on&xdstopw=on&title=\'
+

</div>

 

<div>

escape(document.title) +

</div>

 

<div>

escape(document.title) +

</div>

 

<div>

\'&url=\'+location.href,\'\_blank\',\'height=150,width=500,resizable=yes,scrollbar=no,directory=no,menubar=no,location=no\');
w.focus();\</pre\>

</div>

 

<div>

\'&url=\'+location.href,\'\_blank\',\'height=150,width=500,resizable=yes,scrollbar=no,directory=no,menubar=no,location=no\');
w.focus();\</pre\>

</div>

Zeile 18:

Zeile 18:

 

<div>

Die o.g. URL kann beispielsweise auch dafür verwendet werden, um den
Crawler von einer Webseite aus zu steuern.

</div>

 

<div>

Die o.g. URL kann beispielsweise auch dafür verwendet werden, um den
Crawler von einer Webseite aus zu steuern.

</div>

 

 

−

<div>

Die Beschreibung im YaCy-Forum erfolgte im aufgeführten Thread:
http://www.yacy-forum.de/viewtopic.php?t=1433&highlight=http+localhost+~~8080~~+quickcrawllinkp+html

</div>

\+

<div>

Die Beschreibung im YaCy-Forum erfolgte im aufgeführten Thread:
http://www.yacy-forum.de/viewtopic.php?t=1433&highlight=http+localhost+[8090]{.underline}+quickcrawllinkp+html

</div>

 

 

 

<div>

= Verwendung =

</div>

 

<div>

= Verwendung =

</div>
