Improved termination of timed out remote solr requests to peers.
================================================================

Date: 2017-02-06 12:41:24

``` {style="white-space:pre-wrap;width:81ex"}
Improved termination of timed out remote solr requests to peers.

On timeout, closing remote Solr requests is proper than simply using
Thread.interrupt() that is not effective in most cases. Closing does not
ask commit on remote solr, but release http connections resources and is
more likely to end those threads that can else wait indefinitely.

Other related improvements included :
 - no more marking remote peer as not available when remote search is
interrupted before timeout by the cleanup job.
 - added a short fine log level trace of failing remote solr requests
```
