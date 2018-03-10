Seeking Facebook\'s iPhone app key
==================================

Date: 2016-09-20 01:00:49

![](https://www.jwz.org/images/under_attack_pleas_stand_by_by_heder.png)Dear
Lazyweb, how do I get an OAuth token that impersonates Facebook\'s
official app?

Why? Because I desire to post videos to my business\'s \"page\", and
apparently \"normal\" apps can\'t do that. The official Facebook app has
permissions that you apparently cannot give to yourself.

It used to be possible to impersonate the Facebook iPhone app when
accessing it via the graph API by generating an OAuth token using that
app\'s ID (`6628568379`) and secret
(`c1e620fa708a1d5696fb991c1bde5662`).

After working for years, that token stopped working last week: now those
sessions say \"the user has changed the password\", which is\... a weird
error. So I tried to regenerate it the way I had in the past, by loading
this in a logged-in browser:

`https://graph.facebook.com/oauth/authorize?type=user_agent&client_id=6628568379&redirect_uri=http://www.facebook.com/connect/login_success.html&scope=read_stream`

That ought to redirect to a URL with an `access_token=` on it, but now
it says \"does not look like a valid app ID.\"

So maybe the app ID of the current iPhone app is different? But
`"https://graph.facebook.com/iphone?access_token=..."` suggests not.

And if I run the FB iPhone app through mitmproxy, I can\'t log in, so I
can\'t sniff it. Maybe it\'s doing cert pinning. Who knows.

Any suggestions on how to re-crack this bastard?

[Previously](https://www.jwz.org/blog/2016/03/reverse-engineering-tools/),
[previously](https://www.jwz.org/blog/2013/08/oauth-of-fealty/).
