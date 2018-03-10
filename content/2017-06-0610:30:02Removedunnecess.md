Removed unnecessary finalize implementation.
============================================

Date: 2017-06-06 10:30:02

``` {style="white-space:pre-wrap;width:81ex"}
Removed unnecessary finalize implementation.

On such private classes with limited scope but with frequent instance
creations and removals within the application lifecycle, implementing
the finalize method is particularly unwanted as it decreases the garbage
collector performance.
What's more the Object.finalize() method is now deprecated in the JDK 9
and will eventually disappear from future releases (see
https://bugs.openjdk.java.net/browse/JDK-8177970)
```
