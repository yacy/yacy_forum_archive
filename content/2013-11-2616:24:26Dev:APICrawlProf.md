Dev:APICrawlProfileEditor
=========================

Date: 2013-11-26 16:24:26

[/CrawlProfileEditor\_p.xml: ]{.autocomment} moved explanations from
Dev:API here

← Nächstältere Version

Version vom 26. November 2013, 15:24 Uhr

Zeile 1:

Zeile 1:

 

<div>

= /CrawlProfileEditor\_p.xml =

</div>

 

<div>

= /CrawlProfileEditor\_p.xml =

</div>

−

<div>

~~== Parameters ==~~

</div>

 

 

 

 

\+

<div>

[Crawl profiles are collections of information containing start-url,
crawling-depth and filters which specify each running crawl job. Crawl
profiles can be retrieved as XML:]{.underline}

</div>

 

 

−

<div>

~~== Examples ==~~

</div>

 

−

<div>

</div>

 

−

<div>

~~CrawlProfileEditor\_p.xml~~

</div>

 

 

<div>

\<pre\>

</div>

 

<div>

\<pre\>

</div>

 

<div>

\<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"yes\" ?\>  

</div>

 

<div>

\<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"yes\" ?\>  

</div>

Zeile 46:

Zeile 43:

 

<div>

\</pre\>

</div>

 

<div>

\</pre\>

</div>

 

 

−

<div>

== ~~Used~~ ==

</div>

\+

<div>

[This native PHP example shows how to request a list of all crawl
profiles a peer has loaded.]{.underline}

</div>

−

<div>

~~\* YaCymin~~

</div>

\+

<div>

[\<pre\>]{.underline}

</div>

 

\+

<div>

[\<?php]{.underline}

</div>

 

\+

<div>

[  \$command]{.underline}=[\"CrawlProfileEditor\_p.xml\";]{.underline}

</div>

 

\+

<div>

[  //open connection to peer   ]{.underline}

</div>

 

\+

<div>

[  \$YaCyURL]{.underline}=[\"http://mypeer.tld:8080/\"; ]{.underline}

</div>

 

\+

<div>

[  \$cu]{.underline}=[\$YaCyURL.\$command; ]{.underline}

</div>

 

\+

<div>

[  \$queryServer]{.underline} = [curl\_init(\$cu);   ]{.underline}

</div>

 

\+

<div>

[  curl\_setopt(\$queryServer, CURLOPT\_HEADER, 0);]{.underline}

</div>

 

\+

<div>

[  curl\_setopt(\$queryServer, CURLOPT\_RETURNTRANSFER, 1);]{.underline}

</div>

 

\+

<div>

[  curl\_setopt(\$queryServer, CURLOPT\_USERPWD,\$appID);]{.underline}

</div>

 

\+

<div>

[  \$results = curl\_exec(\$queryServer);]{.underline}

</div>

 

\+

<div>

[  curl\_close(\$queryServer); ]{.underline}

</div>

 

\+

<div>

[  //parse xml\...]{.underline}

</div>

 

\+

<div>

[  \$resultarray=xml2array(\$results); ]{.underline}

</div>

 

\+

<div>

[  //get items only]{.underline}

</div>

 

\+

<div>

[ 
\$items=\$resultarray\[\'crawlProfiles\'\]\[\'crawlProfile\'\];]{.underline}

</div>

 

\+

<div>

[  if (\$items)]{.underline}

</div>

 

\+

<div>

[  {]{.underline}

</div>

 

\+

<div>

[  echo \"\<h1\>Crawl Profiles\</h1\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<table\>\";]{.underline}

</div>

 

\+

<div>

[  foreach (\$items as \$item)]{.underline}

</div>

 

\+

<div>

[  {]{.underline}

</div>

 

\+

<div>

[  if (\$tr==\"ffffff\") {\$tr=\"aaaaaa\";} else
{\$tr=\"ffffff\";}]{.underline}

</div>

 

\+

<div>

[  echo \"\<tr bgcolor=\".\$tr.\"\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'hash\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'name\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'status\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'starturl\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'depth\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'mustmatch\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'mustnotmatch\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo
\"\<td\>\".\$item\[\'crawlingIfOlder\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo
\"\<td\>\".\$item\[\'crawlingDomFilterDepth\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo
\"\<td\>\".\$item\[\'crawlingDomFilterContent\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'DomMaxPages\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'withQuery\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'storeCache\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'indexText\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\<td\>\".\$item\[\'indexMedia\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo
\"\<td\>\".\$item\[\'remoteIndexing\'\].\"\</td\>\";]{.underline}

</div>

 

\+

<div>

[  echo \"\</tr\>\";]{.underline}

</div>

 

\+

<div>

[  }]{.underline}

</div>

 

\+

<div>

[  echo \"\</table\>\";]{.underline}

</div>

 

\+

<div>

[}]{.underline}

</div>

 

\+

<div>

[\</pre\>]{.underline}

</div>

 

 

 

 

 

<div>

\[\[Category: API\]\]

</div>

 

<div>

\[\[Category: API\]\]

</div>
