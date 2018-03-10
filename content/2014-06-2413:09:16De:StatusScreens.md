De:StatusScreensaver
====================

Date: 2014-06-24 13:09:16

corrected port 8080-\>8090

← Nächstältere Version

Version vom 24. Juni 2014, 11:09 Uhr

Zeile 14:

Zeile 14:

 

 

 

<div>

\<pre\>\#!/bin/bash

</div>

 

<div>

\<pre\>\#!/bin/bash

</div>

−

<div>

wget http://user:password\@localhost:~~8080~~/Network.xml -O -
2\>/dev/null \\

</div>

\+

<div>

wget http://user:password\@localhost:[8090]{.underline}/Network.xml -O -
2\>/dev/null \\

</div>

 

<div>

\| grep \"\<ppm\>\" \| sed -e
\"s/.\*\<ppm\>\\(\[0-9\]\*\\)\<\\/ppm\>/\\1/\" \\

</div>

 

<div>

\| grep \"\<ppm\>\" \| sed -e
\"s/.\*\<ppm\>\\(\[0-9\]\*\\)\<\\/ppm\>/\\1/\" \\

</div>

 

<div>

-e \"s/ \*//g\" -e \"s/\\(\[0-9\]\*\\)/current PPM: \\1/\"\</pre\>

</div>

 

<div>

-e \"s/ \*//g\" -e \"s/\\(\[0-9\]\*\\)/current PPM: \\1/\"\</pre\>

</div>

Zeile 20:

Zeile 20:

 

<div>

URLs in den Queues:

</div>

 

<div>

URLs in den Queues:

</div>

 

<div>

\<pre\>\#!/bin/bash

</div>

 

<div>

\<pre\>\#!/bin/bash

</div>

−

<div>

wget http://user:password\@localhost:~~8080~~/xml/queues\_p.xml -O -
2\>/dev/null \\

</div>

\+

<div>

wget
http://user:password\@localhost:[8090]{.underline}/xml/queues\_p.xml -O
- 2\>/dev/null \\

</div>

 

<div>

\| grep \"\<url\>\" \| sed -e \"s/\<url\>//g\" -e \"s/\<\\/url\>//g\" -e
\"s/ \*//g\" \| grep -v \^\$\</pre\>

</div>

 

<div>

\| grep \"\<url\>\" \| sed -e \"s/\<url\>//g\" -e \"s/\<\\/url\>//g\" -e
\"s/ \*//g\" \| grep -v \^\$\</pre\>

</div>

 

 
