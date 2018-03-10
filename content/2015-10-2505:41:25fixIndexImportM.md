fix IndexImportMediawiki\_p servlet\'s refresh header
=====================================================

Date: 2015-10-25 05:41:25

``` {style="white-space:pre-wrap;width:81ex"}
fix IndexImportMediawiki_p servlet's refresh header
add url parameter to make sure no parameter are included in refresh url 
which could cause unwanted restart of import job

see http://mantis.tokeek.de/view.php?id=591 comments
```
