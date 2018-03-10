Fixed unresolved pattern case in search results progress bar.
=============================================================

Date: 2017-03-08 10:27:18

``` {style="white-space:pre-wrap;width:81ex"}
Fixed unresolved pattern case in search results progress bar.

This is a fix for mantis 715 (http://mantis.tokeek.de/view.php?id=715).

A possible path scenario that could leading to this case :
 - YaCy is running low in memory
 - a search is requested
 - before the end of search results rendering, the cleanup job runs and
deletes the running search event from the cache because of short memory
 - then yacysearchitem renders with "-UNRESOLVED_PATTERN-" parameter
values passed to the statistics() JavaScript function
```
