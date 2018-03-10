Introduce additional language setting \"browser/Browser Language\" for ...
==========================================================================

Date: 2016-08-23 00:04:24

``` {style="white-space:pre-wrap;width:81ex"}
Introduce additional language setting "browser/Browser Language" for UI internationalization.
If language is set to "browser" the client/user browser language is used to choose from
available translation.
simply: one users browser speaks English -> YaCy responds in English, other users browser speaks French -> YaCy responds in French.

! To make a translation/language available you have to activate the language once ! 
(or manually use the utility class TranslateAll)
In ConfigBasic.html availabel translations are marked green on setting language=Browser
The client language is determined by http header Accept-Language (checked in DefaultServlet)
```
