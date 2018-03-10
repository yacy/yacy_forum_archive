Fixed regression introduced by commit 9ad4d16
=============================================

Date: 2017-05-02 09:32:04

``` {style="white-space:pre-wrap;width:81ex"}
Fixed regression introduced by commit 9ad4d16

On MediaWiki dump imports, the SurrogateReader was trying to unread too
many bytes, then failing with the following exception :
"java.io.IOException: Push back buffer is full".
```
