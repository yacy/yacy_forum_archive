generalize DateDetection with holiday date rules readily available in...
========================================================================

Date: 2016-10-02 03:19:12

``` {style="white-space:pre-wrap;width:81ex"}
generalize DateDetection with holiday date rules readily available in icu
to make sure current dates are recognized (was fixed to 2014 - 2016)
+ adjust holiday date parser from pattern.match to pattern.find to deal with leading and trailing text
+ moved relative date recognition (morgen, tomorrow) to parseline (used by query parser only), as not working and problematic for indexing
+ add test case for parseline (used by query parser)
```
