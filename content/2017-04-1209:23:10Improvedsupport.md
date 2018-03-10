Improved support for non ASCII chars in local file system URLs
==============================================================

Date: 2017-04-12 09:23:10

``` {style="white-space:pre-wrap;width:81ex"}
Improved support for non ASCII chars in local file system URLs

Creating a MultiProtocolURL instance from a File object and then
retrieving a File with getFSFile() was inconsistent with file paths
containing space or non ASCII chars.
```
