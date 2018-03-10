postpone apicall exec date init until actual call
=================================================

Date: 2016-08-07 05:08:55

``` {style="white-space:pre-wrap;width:81ex"}
postpone apicall exec date init until actual call 
fix for http://mantis.tokeek.de/view.php?id=677
The difference is on scheduling a large number of rss feeds and loading 
is not finished before shutdown of YaCy. The change makes sure not already
loaded RSS will be loaded by the scheduler on next startup.
```
