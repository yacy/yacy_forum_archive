Reduced GeoNames locations memory footprint.
============================================

Date: 2016-12-03 09:05:19

``` {style="white-space:pre-wrap;width:81ex"}
Reduced GeoNames locations memory footprint.

Using String instead of StringBuilder instances in GeonamesLocation
allows to reuse the same immutable objects in the Tagging class.

Measurements with VisualVM and GeoNames 0 enabled (cities with a
population > 1000) :
 - OverArchingLocation retained size :
  - initial : 164 666 830 bytes
  - after refactoring : 97 736 804 bytes
 - AutotaggingLibrary retained size :
  - initial : 354 713 633 bytes
   - after refactoring : 309 718 763 bytes
```
