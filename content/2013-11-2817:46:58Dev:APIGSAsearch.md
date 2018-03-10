Dev:APIGSAsearchresult
======================

Date: 2013-11-28 17:46:58

added GSA api

**Neue Seite**

<div>

== GSA (\'\'Google Search Appliance\'\') Search API ==\
YaCy provides exactly the same result output as the Google Search
Appliance provides in XML format. This is an implementation of the\
\[https://developers.google.com/search-appliance/documentation/68/xml\_reference\#results\_xml
Google Search Protocol Reference Version 6.8: XML Output\] service which
Google provides to their commercial boxes that are rented in thousands
all over the world to index intranets and company data in closed
networks as well for universities etc.\
\
\'\'\'Everyone who is using the Google XML API can instantly migrate to
YaCy by just using the servlet at \'\'/gsa/searchresult\'\' within
YaCy\'\'\', i.e.\
http://localhost:8090/gsa/search?q=joshua&num=10\
\
The result is computed by Solr; in fact this result is just an instance
of the standard Solr select api \[\[Dev:APISolrSelect\|/solr/select\]\]
using a special Solr result writer for the GSA. \'\'The Google API was
implemented as a Solr result writer.\'\'\
\
If you are not forced to, then please do not use the GSA API since it is
bad. \'\'Not the implementation is bad, the specification is bad.\'\'
The result has no facets and you are forced to use XML which is bad if
you have the opportunity to use i.e. json. We recommend to use the yjson
result writer within the solr API which gives you full access to facets
and a simple, standards-compliant (uses the opensearch specification for
naming of properties) result set.

</div>
