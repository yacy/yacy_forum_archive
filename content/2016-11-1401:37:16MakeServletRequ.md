Make ServletRequest implement the standardized HttpServletRequest int...
========================================================================

Date: 2016-11-14 01:37:16

``` {style="white-space:pre-wrap;width:81ex"}
Make ServletRequest implement the standardized HttpServletRequest interface,
to make all readily available information from the original ServletRequest
available to YaCy servlets (without converting data to internal structures).
The implementation of the common interface allows easier integration of
YaCy servlets with the servlet standard (e.g. shared login service with
the servlet container etc.)
```
