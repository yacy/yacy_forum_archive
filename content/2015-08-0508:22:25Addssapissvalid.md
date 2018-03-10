Add /api/validate.json to validate a data source
================================================

Date: 2015-08-05 08:22:25

``` {style="white-space:pre-wrap;width:81ex"}
Add /api/validate.json to validate a data source

Require two parameters : url and source_type

* url : the url to the source
* source_type : a supported source type string. Some source types exist but aren't supported by the validator, since loklak doesn't store its json schema (or xml/rss schema). In such cases a 400 error is thrown

Fixes #101
```
