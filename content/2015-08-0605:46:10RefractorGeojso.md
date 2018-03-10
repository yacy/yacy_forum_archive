Refractor GeojsonPushServlet to reuse some components with AbstractPushServlet
==============================================================================

Date: 2015-08-06 05:46:10

``` {style="white-space:pre-wrap;width:81ex"}
Refractor GeojsonPushServlet to reuse some components with AbstractPushServlet

GeojsonPushServlet can't extend AbstractPushServlet due to its particularity. Nevertheless it can (and it should) reuse some similar steps like saving message & printing report.
```
