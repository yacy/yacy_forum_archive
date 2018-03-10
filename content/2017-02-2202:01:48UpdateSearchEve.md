Update SearchEvent.java
=======================

Date: 2017-02-22 02:01:48

``` {style="white-space:pre-wrap;width:81ex"}
Update SearchEvent.java

Fix NPE on disabled local SolrIndex, occuring on search moving to the 2nd result page.
The debug purpose only setting to disabeling local SolrIndex (System Admin -> Debug Settings) should long term probably be removed from production code.
```
