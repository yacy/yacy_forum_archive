reintroduce special handling of file upload multipart/form-data from HTTPDemon.parseMultipart
=============================================================================================

Date: 2015-12-31 03:04:13

``` {style="white-space:pre-wrap;width:81ex"}
reintroduce special handling of file upload multipart/form-data from HTTPDemon.parseMultipart
- add filename to parameter fieldname
- add filecontent to special parameter fieldname$file
(some servlets use this $file parameter)

fix for http://mantis.tokeek.de/view.php?id=542
```
