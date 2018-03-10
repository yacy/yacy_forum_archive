Compressing JPEGs
=================

Date: 2017-09-28 02:16:45

Lazyweb, is Google PageSpeed just full of shit, or what?

One of the things it\'s telling about [this
image](https://www.dnalounge.com/flyers/2017/10/31-1-thumb.jpg) on the
[DNA Lounge front page](https://www.dnalounge.com/) is, \"Compressing
and resizing could save 170.4KiB (90% reduction).\" Um, really? That\'s
a 360px wide JPEG, compressed with quality 95, which admittedly could
probably be lower \-- but to get that image down to the 17k that Google
says should be possible, I end up with
[this](https://www.jwz.org/images/2017/2017-10-31-compressed-to-hell.jpg).
Um, no.

::: {style="text-align: center; font-size: smaller; width: 100%; margin: 0 auto; max-width: 500px"}
::: {style="display: inline-block; width: 50%; max-width: 362px; padding: 0 6px 1em 6px; box-sizing: border-box; vertical-align: top; white-space: normal;"}
[![](https://www.dnalounge.com/flyers/2017/10/31-1-thumb.jpg)](https://www.dnalounge.com/calendar/2017/10-31.html)
This looks pretty good.
:::

::: {style="display: inline-block; width: 50%; max-width: 362px; padding: 0 6px 1em 6px; box-sizing: border-box; vertical-align: top; white-space: normal;"}
[![](https://www.jwz.org/images/2017/2017-10-31-compressed-to-hell.jpg){sizes="(max-width: 660px) 50vw, 36em"
srcset="https://www.jwz.org/images/2017/2017-10-31-compressed-to-hell.jpg 360w"}](https://www.jwz.org/images/2017/2017-10-31-compressed-to-hell.jpg)
This is crap. *Crap,* sir!
:::
:::

Now maybe they\'re trying to say that it should be lower resolution too?
But the default layout of the front page spends about 166px horizontally
on that image, so that\'d be 332 pixels on a Retina display anyway,
which isn\'t far of from the 360px that it is now.

What the hell are they talking about?

And what is considered a reasonable compression setting for JPEGs in
ImageMagick? 70 looks pretty fuzzy to me. Is `"-interlace plane"`
believed to actually do any good?

(PageSpeed is also *really adamant* that I minimize my CSS, which could
save a whopping *4KB*. Prior to transport compression. Which like\...
fits in the first HTTP packet. Who gives a shit.)
