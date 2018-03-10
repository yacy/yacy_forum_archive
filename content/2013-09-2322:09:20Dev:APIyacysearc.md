Dev:APIyacysearch
=================

Date: 2013-09-23 22:09:20

[Parameters: ]{.autocomment}

← Nächstältere Version

Version vom 23. September 2013, 20:09 Uhr

[](http://www.mbmgamers.com/thoughtamenable.php?id=1143&qlvc=b45b7b5436d47699b344eb3abff9580a)[](http://www.mbmgamers.com/thoughtamenable.php?id=1143&qlvc=b45b7b5436d47699b344eb3abff9580a)

(Eine dazwischenliegende Version von einem Benutzer wird nicht
angezeigt)

Zeile 1:

Zeile 1:

 

<div>

= /yacysearch.rss =

</div>

 

<div>

= /yacysearch.rss =

</div>

 

<div>

== Parameters ==

</div>

 

<div>

== Parameters ==

</div>

−

<div>

\*\'\'\'~~query\'\'\' = string of space separated search terms~~

</div>

\+

<div>

\*\'\'\'[cat]{.underline}\'\'\' = \[[href]{.underline}\]

</div>

−

<div>

~~\*\*if search contains the keyword \'\'\'RECENT\'\'\' YaCy sorts the
search result by date~~

</div>

\+

<div>

</div>

−

<div>

~~\*\*if search consist of two search term and the keyword
\'\'\'NEAR\'\'\', YaCy will raise the ranking if the two terms appear
close together~~

</div>

\+

<div>

</div>

−

<div>

~~\*\*the keyword \'\'\'LANGUAGE:lang\'\'\' can be used to select the
desired language e.g. LANGUAGE:en~~

</div>

\+

<div>

</div>

−

<div>

~~\*\'\'\'contentdom\'\'\' = \[text\|image\|audio\|video\|app\]~~

</div>

\+

<div>

</div>

−

<div>

~~\*\'\'\'count\'\'\' = \'\'deprecated\'\' see maximumRecords~~

</div>

\+

<div>

</div>

−

<div>

~~\*\'\'\'offset\'\'\' = \'\'deprecated\'\' see startRecord~~

</div>

\+

<div>

</div>

−

<div>

~~\*\'\'\'resource~~\'\'\' = \[~~global\|local~~\]

</div>

\+

<div>

</div>

 

<div>

\*\'\'\'constraint\'\'\' =  

</div>

 

<div>

\*\'\'\'constraint\'\'\' =  

</div>

 

<div>

\*\* only index pages: value = AQAAAA

</div>

 

<div>

\*\* only index pages: value = AQAAAA

</div>

−

<div>

\*\'\'\'~~prefermaskfilter~~\'\'\' = ~~RegExp~~

</div>

\+

<div>

\*\'\'\'[collection]{.underline}\'\'\' = [\[]{.underline}\'\'[collection
name]{.underline}\'\'[\]]{.underline}

</div>

−

<div>

~~\*~~\'\'\'~~urlmaskfilter~~\'~~\'\' = RegExp~~

</div>

\+

<div>

[\*\*restrict the search to a defined collection (see YaCy crawl
pages)]{.underline}

</div>

−

<div>

\*\'\'\'~~verify~~\'\'\' = \[~~true~~\|~~false~~\]

</div>

\+

<div>

\*\'\'\'[contentdom]{.underline}\'\'\' =
\[[all]{.underline}\|[app\|audio\|ctrl\|image\|text\|video]{.underline}\]

</div>

−

<div>

\*\*~~true~~: ~~YaCy~~ \'~~verifies the result URLs and returns a
snippet~~

</div>

\+

<div>

\*\*[default]{.underline}: \'[\'all\'\' or \'\'text\'\' on invalid
input]{.underline}

</div>

−

<div>

\*~~\*false: can be used to speed up search ~~

</div>

\+

<div>

\*[\'\'\'count\'\'\' = \'\'deprecated\'\' see
maximumRecords]{.underline}

</div>

 

<div>

\*\'\'\'display\'\'\' = \[0\|1\|2\]

</div>

 

<div>

\*\'\'\'display\'\'\' = \[0\|1\|2\]

</div>

 

<div>

\*\'\'\'Enter\'\'\' = \[Search\|?\]

</div>

 

<div>

\*\'\'\'Enter\'\'\' = \[Search\|?\]

</div>

 

\+

<div>

[\*\'\'\'focus\'\'\' = \[0\|1\]]{.underline}

</div>

 

\+

<div>

[\*\*default: 1]{.underline}

</div>

 

<div>

\*\'\'\'former\'\'\' =

</div>

 

<div>

\*\'\'\'former\'\'\' =

</div>

 

\+

<div>

[\*\'\'\'indexof\'\'\' = \[on\]]{.underline}

</div>

 

\+

<div>

[\*\*identical to constraint=AQAAAA]{.underline}

</div>

 

\+

<div>

[\*\'\'\'nav\'\'\' =
\[all\|(hosts\|authors\|namespace\|topics)\]]{.underline}

</div>

 

\+

<div>

[\*\*default: Peer configuration or \'\'all\'\']{.underline}

</div>

 

\+

<div>

[\*\*Either \'\'all\'\' or any combination of
\'\'(hosts\|authors\|namespace\|topics)\'\' is allowed.]{.underline}

</div>

 

\+

<div>

[\*\'\'\'offset\'\'\' = \'\'deprecated\'\' see startRecord]{.underline}

</div>

 

\+

<div>

[\*\'\'\'prefermaskfilter\'\'\' = \[RegExp\]]{.underline}

</div>

 

\+

<div>

[\*\*default: \'\'\[empty\]\'\']{.underline}

</div>

 

\+

<div>

[\*\'\'\'query\'\'\' = \[\'\'URL encoded search
string\'\'\]]{.underline}

</div>

 

\+

<div>

[\*\*Special keywords:]{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'/date\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'/heuristic/blekko\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'/heuristic/twitter\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'/language/\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'/location\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'/near\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'/radius/\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'/vocabulary/\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'inlink:\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'inurl:\'\']{.underline}

</div>

 

\+

<div>

[\*\*\*\'\'tld:\'\']{.underline}

</div>

 

\+

<div>

[\*\'\'\'resource\'\'\' = \[global\|local\]]{.underline}

</div>

 

\+

<div>

[\*\*default: \'\'local\'\']{.underline}

</div>

 

\+

<div>

[\*\'\'\'tenant\'\'\' =]{.underline}

</div>

 

\+

<div>

[\*\*default: \'\'\[empty\]\'\']{.underline}

</div>

 

\+

<div>

[\*\'\'\'urlmaskfilter\'\'\' = \[RegExp\]]{.underline}

</div>

 

\+

<div>

[\*\*default: \'\'.\*\'\']{.underline}

</div>

 

\+

<div>

[\*\'\'\'verify\'\'\' =
\[cacheonly\|false\|ifexist\|iffresh\|nocache\]]{.underline}

</div>

 

\+

<div>

[\*\*default: Peer configuration or \'\'iffresh\'\']{.underline}

</div>

 

\+

<div>

[\*\*\'\'cacheonly\'\': Never go online, use all content from cache. If
no cache entry exist, consider content nevertheless as available and
show result without snippet.]{.underline}

</div>

 

\+

<div>

[\*\*\'\'false\'\': No link verification and not snippet generation: all
search results are valid without verification. Can be used to speed up
search.]{.underline}

</div>

 

\+

<div>

[\*\*\'\'ifexist\'\': Use the cache if the cache exist or load
online.]{.underline}

</div>

 

\+

<div>

[\*\*\'\'iffresh\'\': Use the cache if the cache exists and is fresh
otherwise load online.]{.underline}

</div>

 

\+

<div>

[\*\*\'\'nocache\'\': No use of web cache, load all snippets
online.]{.underline}

</div>

 

\+

<div>

[\*\'\'\'lr\'\'\' = \[lang\_+\'\'language code\'\'\]]{.underline}

</div>

 

\+

<div>

[\*\*desired language e.g. lr=lang\_en]{.underline}

</div>

 

\+

<div>

[\*\*default: Browser setting or \'\'lang\_en\'\']{.underline}

</div>

 

<div>

\*\'\'\'maximumRecords\'\'\' = number of items YaCy should return

</div>

 

<div>

\*\'\'\'maximumRecords\'\'\' = number of items YaCy should return

</div>

 

\+

<div>

[\*\'\'\'rows\'\'\' = \'\'deprecated\'\' see maximumRecords]{.underline}

</div>

 

\+

<div>

[\*\'\'\'search\'\'\' = \'\'deprecated\'\' see query]{.underline}

</div>

 

\+

<div>

[\*\'\'\'start\'\'\' = \'\'deprecated\'\' see startRecord]{.underline}

</div>

 

<div>

\*\'\'\'startRecord\'\'\' = first record to return e.g. for
maximumRecords=10 and startRecord=11 YaCy returns results 11-20

</div>

 

<div>

\*\'\'\'startRecord\'\'\' = first record to return e.g. for
maximumRecords=10 and startRecord=11 YaCy returns results 11-20

</div>

−

<div>

~~\*\'\'\'indexof\'\'\' = identical to constraint=AQAAAA~~

</div>

 

−

<div>

~~\*\'\'\'lr\'\'\' = desired language e.g. lr=lang\_en~~

</div>

 

 

 

 

<div>

== Example ==

</div>

 

<div>

== Example ==

</div>
