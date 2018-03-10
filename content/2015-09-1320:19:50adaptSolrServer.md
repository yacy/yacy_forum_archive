adapt SolrServerConnector.add to handle error on partial update input document.
===============================================================================

Date: 2015-09-13 20:19:50

``` {style="white-space:pre-wrap;width:81ex"}
adapt SolrServerConnector.add to handle error on partial update input document.
In case of error we deleted the original document and added the new doc to the index.
This is not valid for partial update documents (which contain only a subset of the fields).
Remove the "delete" error handling step.
```
