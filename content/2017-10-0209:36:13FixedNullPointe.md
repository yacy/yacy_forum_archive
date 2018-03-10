Fixed NullPointerException case on \'Browser\' lang selection
=============================================================

Date: 2017-10-02 09:36:13

``` {style="white-space:pre-wrap;width:81ex"}
Fixed NullPointerException case on 'Browser' lang selection

Occurred when English was the only active language, then making the
ConfigBasic.html page unusable until manually modifying the
locale.language setting.
```
