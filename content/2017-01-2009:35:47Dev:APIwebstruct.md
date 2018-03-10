Dev:APIwebstructure
===================

Date: 2017-01-20 09:35:47

Filled webstructure.xml API documentation

← Nächstältere Version

Version vom 20. Januar 2017, 08:35 Uhr

Zeile 1:

Zeile 1:

 

<div>

= /api/webstructure.xml =

</div>

 

<div>

= /api/webstructure.xml =

</div>

−

<div>

== ~~Parameters~~ ==

</div>

\+

<div>

 

</div>

−

<div>

~~\'\'\'latest\'\'\' =~~

</div>

\+

<div>

[The webstructure.xml API retrieves the locally known web links
structure of a specified resource (\"about\" parameter supplied) or the
whole computed links structure since install (no parameter supplied) or
since last start or last call (\"latest\" parameter
supplied).]{.underline}

</div>

−

<div>

\*~~Shows~~ only the ~~recent entries once~~ (~~\'new~~-list~~\'). They
can then be retrieved without parameters~~.

</div>

\+

<div>

 

</div>

−

<div>

== ~~Example~~ ==

</div>

\+

<div>

[Remarks :]{.underline}

</div>

−

<div>

== ~~Elements~~ ==

</div>

\+

<div>

[\* Information detail is limited by some hard-coded  constants :
WebStructureGraph.maxhosts, WebStructureGraph.maxref and
WebStructureGraph.MAX\_PARSED\_ANCHORS]{.underline}

</div>

−

<div>

== ~~Used~~ ==

</div>

\+

<div>

[\* Requesting client must be authenticated (as admin or requesting from
localhost enabled) otherwise results will be empty]{.underline}

</div>

−

<div>

\* ~~Terminal Page~~

</div>

\+

<div>

 

</div>

 

\+

<div>

== [Properties in the http post-arguments]{.underline} ==

</div>

 

\+

<div>

[Calls to the servlet can be made using HTTP GET or POST operation. The
supported parameter keys are:]{.underline}

</div>

 

\+

<div>

\* [about : get]{.underline} only [links structure about]{.underline}
the [resource specified as value. Supported values : host hash, URL
hash, host name or URL]{.underline}

</div>

 

\+

<div>

[\* latest]{.underline} ([ignored when about parameter is valued): get
the structure that have been computed during the current
run]{.underline}-[time of YaCy, and with each next call only an update
to the next]{.underline} list [of references]{.underline}.

</div>

 

\+

<div>

[\* agentName : name of the user agent string used to load the \"about\"
resource]{.underline}

</div>

 

\+

<div>

[\* documentStructure : set to false when you only want the hosts
accumulated references for the \"about\" resource]{.underline}

</div>

 

\+

<div>

 

</div>

 

\+

<div>

== [Result]{.underline} ==

</div>

 

\+

<div>

[The returned xml document contains the following information
:]{.underline}

</div>

 

\+

<div>

[\* in all cases :]{.underline}

</div>

 

\+

<div>

[\*\* accumulated list of outgoing links to other domains (per host
accumulated anchors)\</li\>]{.underline}

</div>

 

\+

<div>

[\* when \"about\" parameter is filled :]{.underline}

</div>

 

\+

<div>

[\*\* accumulated list of incoming links from other domains (per host
accumulated references)\</li\>]{.underline}

</div>

 

\+

<div>

[\*\* detailed list of outgoing links (anchors) from document at
\"about\" URL to references\</li\>]{.underline}

</div>

 

\+

<div>

[\*\* detailed list of incoming links (citations) from other documents
(their references) - reverse link structure\</li\>]{.underline}

</div>

 

\+

<div>

 

</div>

 

\+

<div>

== [Example usages]{.underline} ==

</div>

 

\+

<div>

[\* domain name and index page structure :
http://localhost:8090/api/webstructure.xml?about]{.underline}=[yacy.net]{.underline}

</div>

 

\+

<div>

[\* domain name structure :
http://localhost:8090/api/webstructure.xml?about]{.underline}=[yacy.net&documentStructure]{.underline}=[false]{.underline}

</div>

 

\+

<div>

[\* hosts accumulated structure and specific resource structure :
http://localhost:8090/api/webstructure.xml?about]{.underline}=[http://yacy.net/fr/API.html]{.underline}

</div>

 

\+

<div>

\* [whole locally known hosts web structure :
http://localhost:8090/api/webstructure.xml]{.underline}

</div>

 

\+

<div>

[\* recently locally computed hosts web structure :
http://localhost:8090/api/webstructure.xml?latest=]{.underline}

</div>
