Fixed NullPointerException case on Table init with relative file path.
======================================================================

Date: 2018-01-29 14:00:43

``` {style="white-space:pre-wrap;width:81ex"}
Fixed NullPointerException case on Table init with relative file path.

Can occur for example when running dbtest with relative test table file
name (wihout explicit parent folder).
```
