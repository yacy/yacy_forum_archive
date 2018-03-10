Improved parsing support for OOXML spreadsheets (.xlsx)
=======================================================

Date: 2017-08-21 09:38:20

``` {style="white-space:pre-wrap;width:81ex"}
Improved parsing support for OOXML spreadsheets (.xlsx)

As reported edycop in mantis 765 (
http://mantis.tokeek.de/view.php?id=765 ), parsing of xlsx files was
quite incomplete.
Now properly support "Shared String Table" entry in Office Open XML
spreadsheets, an also detect embedded URLs.

Integrating the Apache poi-ooxml library could be an option for finer
OOXML formats support, but their SAX style parsing example (
http://poi.apache.org/spreadsheet/how-to.html#xssf_sax_api ) tends to
show that a custom SAX handler is still efficient for lightweight and
low memory footprint processing.
```
