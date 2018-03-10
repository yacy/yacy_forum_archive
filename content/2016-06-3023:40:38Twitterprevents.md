Twitter prevents screen locking
===============================

Date: 2016-06-30 23:40:38

![](https://www.jwz.org/images/theclapgy0wl5.gif)If a *hidden* Twitter
window decides to load and invisibly auto-play a video, your screen will
never auto-lock. Proof:

> `% pmset -g assertions | grep PreventUserIdleDisplaySleep   PreventUserIdleDisplaySleep 1   pid 492(Twitter): [0x0002b542000525f7] 02:09:55 PreventUserIdleDisplaySleep named: "com.apple.avkit.disableUserIdleDisplaySleep" `

But at least this idiotic slow-clap is in good company, since [playing
HDMI audio in iTunes does the same fucking
thing.](https://www.jwz.org/blog/2015/11/hdmi-audio-prevents-screen-saver-2/)
