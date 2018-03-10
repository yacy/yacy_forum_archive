Remove redundant code from specialized start scripts.
=====================================================

Date: 2016-12-13 23:40:24

``` {style="white-space:pre-wrap;width:81ex"}
Remove redundant code from specialized start scripts.

Both `bluemix_start.sh` and `heroku_start.sh` have the same exact
start procedure as `start.sh`. The only difference is they both ignore
waiting for loklak to finish starting up and ignore checking for
installation config.

This commit also adds an executable bit to both `bluemix_start.sh` and
`heroku_start.sh`.
```
