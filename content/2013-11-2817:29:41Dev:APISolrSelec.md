Dev:APISolrSelect
=================

Date: 2013-11-28 17:29:41

added Solr select api

**Neue Seite**

<div>

== Solr search API ==\
This is the direct access to the deeply-, embedded
\[http://lucene.apache.org/solr/ Apache Solr Server\] which is used by
YaCy to store document metadata and a search index for the schema as
defined in \[\[Dev:APIIndexSchema\|/IndexSchema\_p.html\]\]. The Solr
Schema can be retrieved in standard Solr-Syntax from the servlet
\[\[Dev:APIschema\|/api/schema.xml\]\]. The Solr interface is very
powerful and can be used in the exact same way as described in the
\[http://wiki.apache.org/solr/SolrQuerySyntax Solr Query Syntax\]. I.e.
an example is:\
http://localhost:8090/solr/select?q=\*:\*&defType=edismax&start=0&rows=3&core=collection1\
Please see the original Apache Solr documentation for all functionality
of that interface. This interface is not only the same, it is identical
because it is attached to the Solr Core directly in the same way as the
original Solr servlet is attached without usage of solrj.\
\
=== Extra Feature: Solr Core Selection ===\
\
You may notice the parameter \'\'core=collection1\'\'. This is special
and it addresses the standard core \'collection1\' which is the default
if you omit the parameter. The second search core for webgraph
descriptions can be retrieved with the parameter \'\'core=webgraph\'\'.\
\
=== Extra Feature: Additional Result Writers for Solr ===\
There is another difference to the standard Solr select API since in
YaCy we provide some more result writers as a standard component. One of
these result writers produce the same output as the
\[Dev:APIyacysearch\|yacysearch.rss and yacysearch.json\] standard YaCy
search servlet.\
The result writer names are \'\'opensearch\'\' and \'\'yjson\'\'; the
\'\'yjson\'\' format is different from the solr-embedded \'\'json\'\'
result writer because it used the same property names as the opensearch
result writer.\
\
That means: the result format of\
http://localhost:8090/solr/select?q=text\_t:joshua&defType=edismax&start=0&rows=10&core=collection1&wt=opensearch\
is identical to\
http://localhost:8090/yacysearch.rss?query=joshua\
\
and the result format of\
http://localhost:8090/solr/select?q=text\_t:joshua&defType=edismax&start=0&rows=10&core=collection1&wt=yjson\
is identical to\
http://localhost:8090/yacysearch.json?query=joshua\
\
..but in both cases the ranking is different, since the solr search uses
a different ranking approach than the YaCy search (which in some depends
on solr)\
\
\
=== Example Code ===\
\
All the examples in the \[\[http://wiki.apache.org/solr/Solrj Solrj
documentation for the \'\'select\'\' servlets\]\] apply. You can use
Solrj to access YaCy\'s embedded Solr. In fact, one part of the YaCy
peer-to-peer remote search actually uses Solrj to retrieve remote search
results from remote YaCy-embedded Solr.

</div>
