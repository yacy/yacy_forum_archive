optimize Translator
===================

Date: 2016-06-05 03:57:08

``` {style="white-space:pre-wrap;width:81ex"}
optimize Translator
- translateFilesRecursive: load translation once (reduce io), return true on complete success
  - remove resulting unused translateFiles() variant
- translate: use StringBuilder parameter (skip toString conversion)
- remove not needed static declaration
- upd some javadoc
```
