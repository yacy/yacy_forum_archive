Eleminate duplication of values for search ResultEntry
======================================================

Date: 2015-05-26 04:15:00

``` {style="white-space:pre-wrap;width:81ex"}
Eleminate duplication of values for search ResultEntry 
by instatiation from URIMetadataNode, by eleminating differentiation of ResultEntry/URIMetadataNode.
- moved remaining ResultEntry functionallity to URIMetadataNode
   - for 1:1 functionallity added a function makeResultEntry() 
- removed ResultEntry 
- refactored related code

Main difference is after makeResultEntry the text_t content is removed and alternative title/url strings for display are calculated.


Main difference left is, that
```
