Improved ErrorCache behavior when switching networks
====================================================

Date: 2016-09-22 09:07:07

``` {style="white-space:pre-wrap;width:81ex"}
Improved ErrorCache behavior when switching networks

Even after network switch, ErroCache was still holding a reference to
the previous Solr cores, thus becoming useless until next YaCy restart.

Initial error cache filling with recent errors from the index was also
missing after the swtich.
```
