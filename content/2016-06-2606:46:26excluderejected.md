exclude rejected results from result count
==========================================

Date: 2016-06-26 06:46:26

``` {style="white-space:pre-wrap;width:81ex"}
exclude rejected results from result count 
  (by using the resultcontainer.size instead of input docList.size)
skip waiting for write-search-result-to-local-index
  (by removing the Thread.join - which will bring a small performance increase)
```
