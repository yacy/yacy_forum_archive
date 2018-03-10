Removed unnecessary crawlingDomFilterDepth hidden field.
========================================================

Date: 2016-10-05 13:48:22

``` {style="white-space:pre-wrap;width:81ex"}
Removed unnecessary crawlingDomFilterDepth hidden field.

It had incorrect "-UNRESOLVED_PATTERN-" value (see  second part of
mantis 691 http://mantis.tokeek.de/view.php?id=691 )

Note : crawlingDomFilterDepth is apparently unused in current (2016)
YaCy code-base. It was also unnecessary because crawlingDomFilterCheck
hidden field is set to "off".
```
