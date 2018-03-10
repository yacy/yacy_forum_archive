enhanced timezone managament for indexed data:
==============================================

Date: 2015-04-15 13:17:23

``` {style="white-space:pre-wrap;width:81ex"}
enhanced timezone managament for indexed data:
to support the new time parser and search functions in YaCy a high
precision detection of date and time on the day is necessary. That
requires that the time zone of the document content and the time zone of
the user, doing a search, is detected. The time zone of the search
request is done automatically using the browsers time zone offset which
is delivered to the search request automatically and invisible to the
user. The time zone for the content of web pages cannot be detected
automatically and must be an attribute of crawl starts. The advanced
crawl start now provides an input field to set the time zone in minutes
as an offset number. All parsers must get a time zone offset passed, so
this required the change of the parser java api. A lot of other changes
had been made which corrects the wrong handling of dates in YaCy which
was to add a correction based on the time zone of the server. Now no
correction is added and all dates in YaCy are UTC/GMT time zone, a
normalized time zone for all peers.
```
