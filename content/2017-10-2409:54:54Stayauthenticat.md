Stay authenticated when going to the search start page.
=======================================================

Date: 2017-10-24 09:54:54

``` {style="white-space:pre-wrap;width:81ex"}
Stay authenticated when going to the search start page.

Otherwise, when authenticated as admin and navigating from search
results or admin pages to the search start page (/index.html), if
nothing is done on that page within HTTP Digest Auth timeout (about
2mn), then search is performed without authentication and so without
extended search features.
```
