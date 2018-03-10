Fixed unresolved pattern on directory entries in HostBrowser.xml api.
=====================================================================

Date: 2017-01-31 09:20:19

``` {style="white-space:pre-wrap;width:81ex"}
Fixed unresolved pattern on directory entries in HostBrowser.xml api.

As described in mantis 725 (http://mantis.tokeek.de/view.php?id=725) the
HostBrowser.xml api directory entries had incorrect count attribute
value. 
This was because the HostBrowser html page and backing template servlet
evolved, but modifications were not reported on the xml api.
```
