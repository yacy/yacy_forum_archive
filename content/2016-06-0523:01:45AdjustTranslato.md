Adjust TranslatorXliff to load default 1st and merge downloaded or modified local translation.
==============================================================================================

Date: 2016-06-05 23:01:45

``` {style="white-space:pre-wrap;width:81ex"}
Adjust TranslatorXliff to load default 1st and merge downloaded or modified local translation.
process 1. load default from locales/*.* 
        2. load and merge(overwrite) from DATA/LOCALE/*.* (can be partial translation as it is merged)
- include all entries from DATA/LOCAL to be edited in Translator servlet
  and save just modifications (instead of full list) to DATA/LOCALE

This shall make it easy to share modifications.
```
