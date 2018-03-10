Dev:APIbookmarksGET
===================

Date: 2014-06-24 13:07:40

corrected port 8080-\>8090

← Nächstältere Version

Version vom 24. Juni 2014, 11:07 Uhr

Zeile 6:

Zeile 6:

 

<div>

=== XBEL ===

</div>

 

<div>

=== XBEL ===

</div>

 

<div>

\* Retrieve all bookmarks as one single XBEL file

</div>

 

<div>

\* Retrieve all bookmarks as one single XBEL file

</div>

−

<div>

 
http://localhost:~~8080~~/xml/bookmarks/get\_bookmarks.xml?display=xbel

</div>

\+

<div>

 
http://localhost:[8090]{.underline}/xml/bookmarks/get\_bookmarks.xml?display=xbel

</div>

 

<div>

\* Retrieve a specific folder as XBEL file

</div>

 

<div>

\* Retrieve a specific folder as XBEL file

</div>

−

<div>

 
http://localhost:~~8080~~/xml/bookmarks/get\_bookmarks.xml?display=xbel&qtype=folders&query=/newspaper

</div>

\+

<div>

 
http://localhost:[8090]{.underline}/xml/bookmarks/get\_bookmarks.xml?display=xbel&qtype=folders&query=/newspaper

</div>

 

<div>

\* Retrieve bookmarks tagged with a specific tag as XBEL file  

</div>

 

<div>

\* Retrieve bookmarks tagged with a specific tag as XBEL file  

</div>

−

<div>

 
http://localhost:~~8080~~/xml/bookmarks/get\_bookmarks.xml?display=xbel&qtype=tagss&query=news

</div>

\+

<div>

 
http://localhost:[8090]{.underline}/xml/bookmarks/get\_bookmarks.xml?display=xbel&qtype=tagss&query=news

</div>

 

<div>

=== XML ===

</div>

 

<div>

=== XML ===

</div>

 

<div>

\* Retrieve all bookmarks as XML posts

</div>

 

<div>

\* Retrieve all bookmarks as XML posts

</div>

−

<div>

  http://localhost:~~8080~~/xml/bookmarks/get\_bookmarks.xml

</div>

\+

<div>

  http://localhost:[8090]{.underline}/xml/bookmarks/get\_bookmarks.xml

</div>

 

 

 

<div>

  \<posts\>

</div>

 

<div>

  \<posts\>

</div>

Zeile 24:

Zeile 24:

 

<div>

=== RSS ===

</div>

 

<div>

=== RSS ===

</div>

 

<div>

\* Retrieve bookmarks as RSS feed

</div>

 

<div>

\* Retrieve bookmarks as RSS feed

</div>

−

<div>

  http://localhost:~~8080~~/xml/bookmarks/get\_bookmarks.xml?display=rss

</div>

\+

<div>

 
http://localhost:[8090]{.underline}/xml/bookmarks/get\_bookmarks.xml?display=rss

</div>

 

 

 

<div>

=== JSON ===

</div>

 

<div>

=== JSON ===

</div>

 

<div>

\* Retrieve page 1 with a maximum of 15 bookmarks per page, tagged with
\'news\', sorted ascending by date  

</div>

 

<div>

\* Retrieve page 1 with a maximum of 15 bookmarks per page, tagged with
\'news\', sorted ascending by date  

</div>

−

<div>

 
http://192.168.2.100:~~8080~~/xml/bookmarks/get\_bookmarks.json?page=1&rp=15&sortname=date&sortorder=asc&query=news&qtype=tags

</div>

\+

<div>

 
http://192.168.2.100:[8090]{.underline}/xml/bookmarks/get\_bookmarks.json?page=1&rp=15&sortname=date&sortorder=asc&query=news&qtype=tags

</div>

 

 

 

<div>

  {

</div>

 

<div>

  {

</div>
