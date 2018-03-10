fixed ReindexSolrBusyThread new and unexpected repeat of same query with
========================================================================

Date: 2017-02-27 23:00:46

``` {style="white-space:pre-wrap;width:81ex"}
fixed ReindexSolrBusyThread new and unexpected repeat of same query with
low number of found documents - by adding additional end condition to 
remove processed query with number of found docs <= process-chunck-size.

Noticed on query h4_txt:[* TO *], found 21, process 21, call of commit happend
but on next cycle same query again 21 docs found (while h4_txt was removed 
from schema and committed inputdocuments).
```
