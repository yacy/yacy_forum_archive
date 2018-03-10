Reduced locations vocabulary memory footprint.
==============================================

Date: 2016-12-05 10:57:37

``` {style="white-space:pre-wrap;width:81ex"}
Reduced locations vocabulary memory footprint.

Reduced this vocabulary memory usage :
 - by using only one map term2entries instead of two maps having the
same key set
 - by generating the location object links on the fly using the
GeoLocation data instead of storing many duplicates of string prefix
"http://www.openstreetmap.org/?lat="
 
Measurements with VisualVM and GeoNames 0 enabled (cities with a
population > 1000) :
 - AutotaggingLibrary retained size :
  - initial : 309 718 763 bytes
  - after refactoring : 159 224 641 bytes
```
