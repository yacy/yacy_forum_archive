Use loaderDispatcher instead of HTTPClient to download releases.
================================================================

Date: 2016-12-16 20:38:54

``` {style="white-space:pre-wrap;width:81ex"}
Use loaderDispatcher instead of HTTPClient to download releases.

The default redirection strategy when using directly HTTPClient is
incorrect when redirection is cross host (the original Host header is
still sent when requesting the redirected location).

YaCy LoaderDispatcher handles redirections properly, thus release
archive files using redirected URLs (such as the URLs on a GitHub
Release page) are successfully downloaded.
```
