introduced three new indexes: mirrors for messages that had been created
========================================================================

Date: 2016-06-24 14:02:22

``` {style="white-space:pre-wrap;width:81ex"}
introduced three new indexes: mirrors for messages that had been created
within one hour, one day and one week. These three indexes are used to
search in when a user searches: first the one-hour index is tried, then,
if not sufficient results have been returned, the one-day index and so
on. This process shall ensure that the overall index should be not too
large, but be searchable as fail-over for rare search words.
TODO: removal of old entries when these indexes fill up.
```
