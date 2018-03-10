Dev:APIyacysearch
=================

Date: 2013-09-23 21:14:30

[Parameters: ]{.autocomment}

← Nächstältere Version

Version vom 23. September 2013, 19:14 Uhr

Zeile 13:

Zeile 13:

 

<div>

\*\'\'\'prefermaskfilter\'\'\' = RegExp

</div>

 

<div>

\*\'\'\'prefermaskfilter\'\'\' = RegExp

</div>

 

<div>

\*\'\'\'urlmaskfilter\'\'\' = RegExp

</div>

 

<div>

\*\'\'\'urlmaskfilter\'\'\' = RegExp

</div>

−

<div>

\*\'\'\'verify\'\'\' = \[~~true~~\|false\]

</div>

\+

<div>

\*\'\'\'verify\'\'\' =
\[[cacheonly]{.underline}\|false[\|ifexist\|iffresh\|nocache]{.underline}\]

</div>

−

<div>

\*\*~~true~~: ~~YaCy \'verifies the result URLs~~ and ~~returns a~~
snippet

</div>

\+

<div>

\*\*[cacheonly]{.underline}: [Never go online, use all content from
cache. If no cache entry exist, consider content nevertheless as
available]{.underline} and [show result without]{.underline}
snippet[.]{.underline}

</div>

−

<div>

\*\*false: ~~can~~ be used to speed up search

</div>

\+

<div>

\*\*false: [No link verification and not snippet generation: all search
results are valid without verification. Can]{.underline} be used to
speed up search[.]{.underline}

</div>

 

\+

<div>

[\*\*ifexist: Use the cache if the cache exist or load
online.]{.underline}

</div>

 

\+

<div>

[\*\*iffresh: Use the cache if the cache exists and is fresh otherwise
load online.]{.underline}

</div>

 

\+

<div>

[\*\*nocache: No use of web cache, load all snippets
online.]{.underline}

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
