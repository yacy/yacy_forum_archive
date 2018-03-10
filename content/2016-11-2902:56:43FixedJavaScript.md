Fixed JavaScript error \"hs.htmlExpand is not a function\".
===========================================================

Date: 2016-11-29 02:56:43

``` {style="white-space:pre-wrap;width:81ex"}
Fixed JavaScript error "hs.htmlExpand is not a function".

This error occurs on /ConfigSearchPage_p.html and on search results page
when Metadata links are enabled.

The fix was to remove unnecessary use of hs.htmlExpand() which is now
part of highslide-full.js library file, currently not distributed with
YaCy (only includes highslide.js). The Metadata links work correctly and
the initial dynamic expansion offered by htmlExpand() did not bring much
usability.
```
