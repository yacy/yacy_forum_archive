reduced translog flush limit drastically (default is 512mb) to 8mb. This
========================================================================

Date: 2016-01-07 13:39:50

``` {style="white-space:pre-wrap;width:81ex"}
reduced translog flush limit drastically (default is 512mb) to 8mb. This
will reduce the performance but will also dramatically reduce start-up
time in case of a recovery. Current recovery times had been over one
hour which is too long to be acceptable for monitoring.
```
