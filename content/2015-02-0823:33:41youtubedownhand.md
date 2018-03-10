youtubedown handles 1080p and 4K now
====================================

Date: 2015-02-08 23:33:41

I updated
[![](http://www.jwz.org/images/under_attack_pleas_stand_by_by_heder.png)youtubedown](http://www.jwz.org/hacks/#youtubedown)
to support 1080p and 4K video. Let me know if it breaks.

Some time last year, Youtube stopped serving up usable videos in any
resolution higher than 720p. They used to offer 1080p and 4K (formats 37
and 38) but those are no longer offered. Apparently the new party line
is that for anything higher than 720p, you are expected to download a
1080p video stream that has no audio in it, and a separate audio stream
that has no video in it, and mux them on the client side.

Which is convenient and awesome.

So now youtubedown does that, if you have `ffmpeg` installed. If you
don\'t have `ffmpeg`, or if you specify `--no-mux`, you max out at 720p
like before.

[Previously](http://www.jwz.org/blog/2013/08/another-day-another-cipher-change/).
