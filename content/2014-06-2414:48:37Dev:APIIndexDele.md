Dev:APIIndexDeletion
====================

Date: 2014-06-24 14:48:37

created deletion guide

**Neue Seite**

<div>

= Index Deletion API =\
Documents in the Solr index can be deleted using this servlet. To delete
a single url, call an expression like the following:\
\
\<pre\>\
http://localhost:8090/IndexDeletion\_p.html?engage-querydelete=&querydelete=sku:\"http://microsoft.com/\"\
\</pre\>\
\
Using a command-line script, you would call i.e. (using curl)\
\<pre\>\
curl -s
\"http://localhost:8090/IndexDeletion\_p.html?engage-querydelete=&querydelete=sku:\\\"http://microsoft.com/\\\"\"
\> /dev/null\
\</pre\>\
\
The parameter options are explained below in detail.\
\
{\| style=\"color:black; background-color:\#efefef;\" cellpadding=\"20\"
cellspacing=\"0\" border=\"0\"\
\|\'\'\'engage-querydelete\'\'\'\
\|(no value needed) - this key must be present to trigger a deletion
using the property \'querydelete\'\
\|-\
\|\'\'\'querydelete\'\'\'\
\|This must be a solr query term. To find appropriate field names, have
a look at the Solr Schema editor /IndexSchema\_p.html. The field name
for the url is \'sku\'. Conjunctions and disjunctions are possible using
the work AND and OR (in uppercase letters). For a complete guide to Solr
query terms, please see the
\[https://wiki.apache.org/solr/SolrQuerySyntax Solr Query Syntax\].\
\|-\
\|}\
\
\[\[Category: API\]\]

</div>
