Apply consistent behavior on HTTP resource size exceeding limit.
================================================================

Date: 2017-06-30 01:13:47

``` {style="white-space:pre-wrap;width:81ex"}
Apply consistent behavior on HTTP resource size exceeding limit.

On content size known from HTTP headers, terminates connection faster
and improves error reports quality by reporting relevant message
"Content to download exceed maximum value..." rather than previously "no
response (NULL) for url...".
```
