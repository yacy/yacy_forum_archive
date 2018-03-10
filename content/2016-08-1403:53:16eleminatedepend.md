eleminate dependency on file-extension in storeDocument but use supported mime-type
===================================================================================

Date: 2016-08-14 03:53:16

``` {style="white-space:pre-wrap;width:81ex"}
eleminate dependency on file-extension in storeDocument but use supported mime-type
to also support handling of urls w/o corresponding file-extension.
For this refactor use of document.getParserObject() to alway return a Parser (for clean logic)
and define/move the scraperObject as local var of AbstractParser.
Adjust related calls to getParserObject (where actually a scraperObject is wanted).
Addionally skip appending url token to parsed text for dht metadata entries 
(by default returned as result by rwi index).
```
