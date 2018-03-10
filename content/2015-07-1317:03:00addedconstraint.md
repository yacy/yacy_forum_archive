added constraint option for /location to select for special sources.
====================================================================

Date: 2015-07-13 17:03:00

``` {style="white-space:pre-wrap;width:81ex"}
added constraint option for /location to select for special sources.
The option can be attached to /location as single value, i.e.:

q=biergarten /location=USER

would select all beer gardens where a user annotated the location with a
rich-tweet. Compare with:

q=biergarten /location=REPORT
(i.e. for IoT locations) and
q=biergarten /location=ANNOTATION
for auto-discovered coordinates when a location mame is given in the
message text.

The source attribute can also be given as fifth parameter if four bbox
values are given as option to /location, i.e.:
/location=1.2,3.4,5.6,7.8,USER
```
