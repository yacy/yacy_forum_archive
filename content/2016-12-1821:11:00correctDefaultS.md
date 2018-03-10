correct DefaultServlet resource pathinContext calculation
=========================================================

Date: 2016-12-18 21:11:00

``` {style="white-space:pre-wrap;width:81ex"}
correct DefaultServlet resource pathinContext calculation
exclude servletPath option as resources are always relative to htroot 
or htdocs, the change reflects this.
Theoretically it and the recent adjustments arcording relative urls 
allows to configure the instance to be configurable in a path other as 
root (/)
```
