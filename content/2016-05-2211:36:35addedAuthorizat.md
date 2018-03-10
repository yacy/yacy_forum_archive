added Authorization object to the service call and made an abstraction
======================================================================

Date: 2016-05-22 11:36:35

``` {style="white-space:pre-wrap;width:81ex"}
added Authorization object to the service call and made an abstraction
of the Post object, which is now in the Query class. This caused that
all servlets had to be modified.
Now the class AbstractAPIHandler is able to handle user access rights.
That class gets an APIServiceLevel object when asked by
AbstractAPIHandler for getCustomServiceLevel. Therefore we can handle
all authorization tasks at a central place.
```
