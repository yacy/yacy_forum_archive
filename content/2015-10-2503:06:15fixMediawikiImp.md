fix MediawikiImporter for bz2 dump
==================================

Date: 2015-10-25 03:06:15

``` {style="white-space:pre-wrap;width:81ex"}
fix MediawikiImporter for bz2 dump
skip reading bz2 file magicbyte to identify bz2 format as inputstream reset would be required. Common compress reads and checks the magicbytes internally and throws ioexception if wrong, making preread obsolete.
```
