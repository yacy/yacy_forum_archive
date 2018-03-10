renamed authentication value fields, the access to accounts is now like:
========================================================================

Date: 2015-05-28 17:48:16

``` {style="white-space:pre-wrap;width:81ex"}
renamed authentication value fields, the access to accounts is now like:

write:
http://localhost:9100/api/account.json?action=update&data={%22screen_name%22:%22myaccount%22,%22oauth_token%22:%221x3%22,%22oauth_token_secret%22:456,%22source_type%22:%22TWITTER%22}
read:
http://localhost:9100/api/account.json?screen_name=myaccount
```
