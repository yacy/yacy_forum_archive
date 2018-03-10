Fixed StringIndexOutOfBoundsException case.
===========================================

Date: 2017-05-09 18:32:47

``` {style="white-space:pre-wrap;width:81ex"}
Fixed StringIndexOutOfBoundsException case.

Revealed by commit c77e43a : the exception was then thrown when indexing
pages containing mailto: scheme URL links with the Solr Webgraph core
enabled.
Fixed the error case and restored filtering on mailto links in
Document.resortLinks() as these URLs still should not appear in
Document.hyperlinks.
```
