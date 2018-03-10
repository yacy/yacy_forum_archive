fix HeaderFramework.mime() to strip charset parameter.
======================================================

Date: 2015-12-20 06:44:16

``` {style="white-space:pre-wrap;width:81ex"}
fix HeaderFramework.mime() to strip charset parameter.
Differentiate mime() and getContentType() which gives the raw header field.
This improves parser detection if charsets are included in http content-type field.
```
