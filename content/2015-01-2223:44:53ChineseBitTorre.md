Chinese BitTorrent, the gift that keeps on giving
=================================================

Date: 2015-01-22 23:44:53

[WAT.](http://serverfault.com/questions/656093/mod-security-block-requests-by-http-host-header)

> After a bit of logging and searching I found out that some Chinese ISP
> (probably CERNET according to the results of whatsmydns.net) and some
> Turkish ISP (probably TTNET) respond to dns queries such as
> a.tracker.thepiratebay.org with various IPs that have nothing to do
> with piratebay or torrents. In other words they seem to do some kind
> of DNS Cache Poisoning for some bizarre reason.
>
> So hundreds (if not thousands) of bittorrent clients on those
> countries make tons of \'announces\' to my webservers which result
> pretty much in a DDoS attack filling up all Apache\'s connections.

So basically, entire countries\' worth of porn hounds randomly start
hammering on my server all at once, even though no BitTorrent traffic
has ever passed to or from the network it\'s on, because for some
unknown reason, the now-long-defunct piratebay tracker sometimes
resolves to *my* IP address. Hooray.

This (possibly) mitigates the problem somewhat, by returning an actual
BitTorrent error message to the clients so they stop retrying sooner:

> `<Location ~ "^/announc">   ErrorDocument 404 "d14:failure reason13:not a tracker8:retry in5:nevere"</Location>`{style="font-size:smaller"}

We had previously blackholed the entire Chinese IP space because of
this, but we missed some.

Hi, how\'s your day going?
