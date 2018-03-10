replaced generation of json with
================================

Date: 2016-05-13 16:10:30

``` {style="white-space:pre-wrap;width:81ex"}
replaced generation of json with
com.fasterxml.jackson.databind.ObjectMapper with toString method in
JSONObject. This caused a domino effect where it was necessary to
replace almost all appearances of Map with JSONObject.
Extensive testing was done, but this code base should now be considered
unstable. Please use with care.
```
