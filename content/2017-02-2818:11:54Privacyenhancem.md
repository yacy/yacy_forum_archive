Privacy enhancement : added settings to control referrer policy.
================================================================

Date: 2017-02-28 18:11:54

``` {style="white-space:pre-wrap;width:81ex"}
Privacy enhancement : added settings to control referrer policy.

HTTP "Referer" header sent by the browser when using YaCy can now be
controlled either with the referrer meta tag as a global policy, or only
for search result links by adding the attribute rel="noreferrer".

To improve privacy with the less possible regressions, the default is
set as meta tag with value "origin-when-cross-origin" : internal YaCy
links behavior is not affected, but when visiting external websites
referrer url is not empty but stripped from query parameters and path.

Older browsers, Safari, MS IE and Edge do not support the referrer meta
tag, so the standard but less flexible noreferrer link type can also be
enabled as an alternative.

User-friendly settings page to be implemented.
```
