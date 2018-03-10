replaced elasticsearch XContentParser with jackson jsonMapper to remove
=======================================================================

Date: 2015-07-30 05:47:12

``` {style="white-space:pre-wrap;width:81ex"}
replaced elasticsearch XContentParser with jackson jsonMapper to remove
dependency on elasticsearch as json reader. This may help to enhance
reusability of the loklak classes outside of elasticsearch projects.
```
