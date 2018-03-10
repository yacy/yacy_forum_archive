fix RuntimeException in ConfigRobotsTxt\_p in intranet mode
===========================================================

Date: 2016-05-27 17:30:17

``` {style="white-space:pre-wrap;width:81ex"}
fix RuntimeException in ConfigRobotsTxt_p in intranet mode
due to getIP returning null, by removing redundant property setting of "clientname"
which is globally set by template engine
```
