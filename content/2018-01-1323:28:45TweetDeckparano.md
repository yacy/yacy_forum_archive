TweetDeck paranoia
==================

Date: 2018-01-13 23:28:45

::: {style=" font-size: smaller;text-align: right; width: 50%; max-width: 612px; margin: 0 0 1em 1em; white-space: nowrap; float: right;"}
::: {style="display: inline-block; width: 100%; max-width: 614px; padding: 0 6px 1em 6px; box-sizing: border-box; vertical-align: top; white-space: normal; text-align: center;"}
![](https://www.jwz.org/images/2018/spyware-concept-picture-id494600583.jpg){sizes="(max-width: 660px) 50vw, 36em"
srcset="https://www.jwz.org/images/2018/spyware-concept-picture-id494600583.jpg 612w, https://www.jwz.org/images/scaled/360/2018/spyware-concept-picture-id494600583.jpg 360w"}*Obligatory
hax0r stock photo*
:::
:::

Dear Lazyweb, is TweetDeck spying on my web browser?

I use TweetDeck because it\'s the only workable way to manage multiple
Twitter accounts.

Recently it has been crashing a lot. It crashes at pretty random times,
but only occasionally when Tweetdeck is the front app. It doesn\'t
*usually* crash when I\'m scrolling down the list. Usually it crashes
when some other app is selected, like when I\'ve clicked a link and it
opens in Safari.

But now I\'ve noticed that it most often crashes when I\'m in Safari,
haven\'t used Tweetdeck at all recently, and I open or close a Safari
window\... *Right then* is when Tweetdeck crashes. Exactly then.

So now I suspect that Tweetdeck is using AppleScript to monitor all the
URLs I load in Safari, and presumably is phoning home with them.

Anyone know how to prove, monitor or prevent this? I don\'t know how
you\'d log or MITM AppleScript IPC.

This behavior would not be unprecedented for such an ethical and
trustworthy company as Twitter: remember when they got busted phoning
home with [all of the applications installed on your
iPhone](https://www.jwz.org/blog/2014/11/time-to-uninstall-the-twitter-app/)
to \"better improve your advertising experience\"? Yeah, they\'d totally
do this.

[Previously](https://www.jwz.org/blog/2017/12/even-my-own-bank-is-canvas-fingerprinting-me/),
[previously](https://www.jwz.org/blog/2014/11/time-to-uninstall-the-twitter-app/),
[previously](https://www.jwz.org/blog/2017/11/shadow-profiles/),
[previously](https://www.jwz.org/blog/2017/10/put-the-ad-network-surveillance-state-to-work-for-you/),
[previously](https://www.jwz.org/blog/2015/10/verizon-has-quietly-made-its-tracking-supercookies-a-lot-more-powerful/),
[previously](https://www.jwz.org/blog/2017/01/twitter-access-control-via-post-it-note/),
[previously](https://www.jwz.org/blog/2017/03/signal-leaks-your-phone-number-to-everyone-in-your-contacts/).
