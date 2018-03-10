Complete harmonization RequestHeader getCookie with std ServletRequest
======================================================================

Date: 2017-01-02 03:04:21

``` {style="white-space:pre-wrap;width:81ex"}
Complete harmonization RequestHeader getCookie with std ServletRequest
to use javax.servlet.http.Cookie parameters.
Depreciate now obsolete getHeaderCookies.
Adjust setting of MaxAge to spec if >= 0 otherwise keep default.
```
