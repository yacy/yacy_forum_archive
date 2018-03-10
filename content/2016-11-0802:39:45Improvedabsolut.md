Improved absolute URLs rendering in OpenSearch desc and RSS feeds.
==================================================================

Date: 2016-11-08 02:39:45

``` {style="white-space:pre-wrap;width:81ex"}
Improved absolute URLs rendering in OpenSearch desc and RSS feeds.

When the peer is behind a reverse proxy providing SSL/TLS encryption,
the rendered absolute URLs should start with https when the user browser
requested https : added limited support to the X-Forwarded-Proto HTTP
header notably provided on Heroku platform.
Also added some unit tests.
```
