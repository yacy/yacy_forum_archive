refactor namespace navigator as part of navigatorplugin map, this allows
========================================================================

Date: 2016-11-01 04:38:47

``` {style="white-space:pre-wrap;width:81ex"}
refactor namespace navigator as part of navigatorplugin map, this allows
the navigator to include counts all matches (rwi+fulltext).
Fixing also unresolved_pattern in navigators title (of the counter)
The use of inurl: query modifier as filter has not been changed keeping
it as soft (unsharp) filter facet.

Upd StringNavigator to prevent empty string form multivalued solr fields,
removed date value conversion (better handled elsewhere, not need here).
```
