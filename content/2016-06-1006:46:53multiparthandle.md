multipart handler now avoids buffering of POSTed content in a temporary
=======================================================================

Date: 2016-06-10 06:46:53

``` {style="white-space:pre-wrap;width:81ex"}
multipart handler now avoids buffering of POSTed content in a temporary
file, if the file size is not too large, to avoid IO.
```
