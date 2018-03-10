expand initRemoteCrawler() to terminate worker threads if called to deactivate
==============================================================================

Date: 2016-01-28 23:14:09

``` {style="white-space:pre-wrap;width:81ex"}
expand initRemoteCrawler() to terminate worker threads if called to deactivate
remote crawl.
On startup we save the resources for remote crawler if disabled. Once started
threads are running idle after disable remote crawl. Now threads are terminated
to save the resources also while disabeling during runtime.
+ remove empty class Channels
```
