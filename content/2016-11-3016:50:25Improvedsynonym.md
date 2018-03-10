Improved synonyms memory footprint.
===================================

Date: 2016-11-30 16:50:25

``` {style="white-space:pre-wrap;width:81ex"}
Improved synonyms memory footprint.

The idea is to avoid unnecessary String objects duplication for the same
words. Particularly efficient with the large moby thesaurus.

Memory footprint measurements with VisualVM :
 - openthesaurus_de_yacy :
    - initial : 19 443 796 bytes
    - after refactoring : 18 012 606 bytes

 - mobythesaurus_en_yacy :
    - initial : 343 453 904 bytes
    - after refactoring : 173 843 780 bytes

 - thesaurus_ru_yacy :
    - initial : 3 800 706 bytes
    - after refactoring : 3 466 612 bytes

 - de + en + ru : 
    - initial : 366 603 450 bytes
    - after refactoring : 195 015 914 bytes
```
