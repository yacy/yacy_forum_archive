Reverse engineering tools
=========================

Date: 2016-03-13 06:24:38

![](https://www.jwz.org/images/under_attack_pleas_stand_by_by_heder.png)Dear
Lazyweb: What are reasonable reverse engineering tools for web sites?

It seems like every few months I find myself cracking the login and
upload or download process on some site \-- sorry, some \"web
application\". Invariably they either don\'t provide an API, or their
API is wholely inadequate. The \"new web\" doesn\'t want you to script
it, because that might prevent them from forcing lock-in on you. They
all want to be titans of the industry like Compuserve or AOL, apparently
not having heard about this little thing called \"The Internet\" that
got really popular for a minute back in the 90s.

So to do the things I want to do, I often have to crack their
undocumented protocols and halfassed security measures. I don\'t enjoy
it, but for my sanity and out of self defense, I do it a lot. [\"Nation
Suddenly Realizes This Just Going To Be A Thing That Happens From Now
On\"](http://www.theonion.com/article/nation-suddenly-realizes-this-just-going-to-be-a-t-30195).

The kind of discoveries I end up needing to make usually look like:

-   Their OAuth \"application\" API is inadequate and intentionally
    crippled, so let\'s go straight for the web login page and get a
    session cookie.
-   Oh look, here\'s the magic URL you are squirting JSON data down.
-   Oh, but the arguments to that URL are signed.
-   Oh, here\'s the signing key you embedded in the code but tried to
    hide.
-   (And you\'re sniffing user agents. Aw, that\'s cute.)

I don\'t have proper tools to easily do the sorts of things I need to do
to solve these problems. I mean, I manage, obviously, but it sucks. Here
are the kind of questions I find myself asking that are harder to answer
than they should be:

-   This form\'s \"Submit\" button isn\'t actually a form element, and
    the source doesn\'t have an `onclick` handler on it. Something
    somewhere else has installed a handler \...somewhere\... so that
    when I click it, a JS function runs and a URL gets loaded. What
    function? What URL?
-   Clicking this thing reads and writes a bunch of data to random URLs
    via `XMLHttpRequest`, then does a redirect. What URLs did it load
    and what did it send and recieve? Sometimes I can answer this
    question using the Resources or Timeline panel in Safari\'s
    inspector, but as far as I can tell, the intermediate data vanishes
    from the timeline as soon as the top-level URL changes, or the DOM
    gets zeroed out, or something. I don\'t know. I just know that I
    can\'t see a record of URLs being loaded that I know were loaded.
    Mozilla and Firebug don\'t seem to be any better than Safari in this
    respect. \"Oh, the document is gone, you must not care about it any
    more.\"
-   This page does some Javascript contortions and eventually emits a
    `<video>` tag and configures it via JS. Eventually that tag
    initiates network activity. What URL is it loading? It doesn\'t show
    up in the inspector. It is happening out-of-process?
-   A URL is being loaded at the bottom of a giant stack of obfuscated,
    minimized Javascript. What\'s the call stack? Basically: if I lived
    in a world where \"javascript debugger\" was a thing that actually
    existed (ha ha ha), how do I set a breakpoint on any network
    activity?

I could use mitmproxy and Wireshark for some of this, but that\'s a huge
pain in the ass, and more heavy-handed that I usually need. Also
Wireshark is awful (it always leaves me thinking \"How was this supposed
to be any better than tcpdump?\") It makes much more sense to intercept
this stuff inside the browser. All the information is in there since
it\'s the thing initiating contact with the server.

[Previously](https://www.jwz.org/blog/2016/01/1982-burgertime-drm-was-hard-core/),
[previously](https://www.jwz.org/blog/2015/05/flickr-download-counter-countermeasures-applied/),
[previously](https://www.jwz.org/blog/2014/03/they-want-to-lock-everyone-into-everything-just-like-everyone-else/),
[previously](https://www.jwz.org/blog/2014/10/i-have-no-joke-here-i-just-like-saying-advanced-demuffin/),
[previously](https://www.jwz.org/blog/2013/08/oauth-of-fealty/),
[previously](https://www.jwz.org/blog/2013/10/w3c-green-lights-adding-drm-to-the-webs-standards/),
[previously](https://www.jwz.org/blog/2012/11/1994-called/).
