ffmpeg volumedetect
===================

Date: 2016-08-23 23:28:16

Dear Lazyweb,

I need to detect the average volume of the left and right channels of an
MP3, considered separately (e.g., to detect when one channel is louder
than the other).

The `ffmpeg volumedetect` filter *really, really* wants to work on both
channels at once. I thought maybe something like this would work, but it
is still averaging the two of them, and producing the same output twice:

> `ffmpeg -hide_banner -i IN.mp3 -filter_complex 'channelsplit=channel_layout=stereo; [0:0:0]volumedetect; [0:0:1]volumedetect' -f null /dev/null`

Any suggestions?

I can do it by writing a temporary file with each channel and then
examining them again, but that\'s a lot slower because these are really
big files. So I\'d rather do it in one pass.
