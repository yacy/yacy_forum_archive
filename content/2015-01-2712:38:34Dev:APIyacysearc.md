Dev:APIyacysearch
=================

Date: 2015-01-27 12:38:34

[Search Interface: ]{.autocomment} added examples

← Nächstältere Version

Version vom 27. Januar 2015, 11:38 Uhr

Zeile 1:

Zeile 1:

 

<div>

= Search Interface =

</div>

 

<div>

= Search Interface =

</div>

 

<div>

The main YaCy search page is at /index.html, but all search results are
presented on the result page at /yacysearch.html. That page provides the
visual results, but can also be used for technical search requests using
an XML or JSON output format. For the search query we use the
\[http://www.loc.gov/standards/sru/ SRU\] (Search/Retrieve via URL)
schema and for the XML result format we use
\[http://www.opensearch.org/Specifications/OpenSearch/1.1/Draft\_5
opensearch\] schema which is an extension of RSS. Therefore, YaCy search
results are readable with any RSS reader right out of the box. To get
this output format, just click on the \'RSS\' box in the upper right of
the search result page or replace \'html\' with \'rss\' in the result
URL.

</div>

 

<div>

The main YaCy search page is at /index.html, but all search results are
presented on the result page at /yacysearch.html. That page provides the
visual results, but can also be used for technical search requests using
an XML or JSON output format. For the search query we use the
\[http://www.loc.gov/standards/sru/ SRU\] (Search/Retrieve via URL)
schema and for the XML result format we use
\[http://www.opensearch.org/Specifications/OpenSearch/1.1/Draft\_5
opensearch\] schema which is an extension of RSS. Therefore, YaCy search
results are readable with any RSS reader right out of the box. To get
this output format, just click on the \'RSS\' box in the upper right of
the search result page or replace \'html\' with \'rss\' in the result
URL.

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[An example path for a search query is]{.underline}

</div>

 

\+

<div>

[/yacysearch.rss?query=freedom&resource=global&urlmaskfilter=.\*&prefermaskfilter=&nav=all]{.underline}

</div>

 

\+

<div>

[The api can also return JSON using]{.underline}

</div>

 

\+

<div>

[/yacysearch.json?query=freedom&resource=global&urlmaskfilter=.\*&prefermaskfilter=&nav=all]{.underline}

</div>

 

\+

<div>

[i.e. try
http://localhost:8090/yacysearch.rss?query=freedom&resource=global&urlmaskfilter=.\*&prefermaskfilter=&nav=all
or
http://localhost:8090/yacysearch.json?query=freedom&resource=global&urlmaskfilter=.\*&prefermaskfilter=&nav=all]{.underline}

</div>

 

 

 

<div>

== GET-Parameters for http Requests ==

</div>

 

<div>

== GET-Parameters for http Requests ==

</div>
