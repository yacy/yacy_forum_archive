En:MonitoringYaCyWithGanglia
============================

Date: 2014-06-24 13:10:57

corrected port 8080-\>8090

← Nächstältere Version

Version vom 24. Juni 2014, 11:10 Uhr

Zeile 23:

Zeile 23:

 

<div>

     def handler(name):

</div>

 

<div>

     def handler(name):

</div>

 

<div>

         try:

</div>

 

<div>

         try:

</div>

−

<div>

             x =
parse(urlopen(\"http://localhost:~~8080~~/Network.xml\"))

</div>

\+

<div>

             x =
parse(urlopen(\"http://localhost:[8090]{.underline}/Network.xml\"))

</div>

 

<div>

             return
convert(x.getElementsByTagName(\"your\")\[0\].getElementsByTagName(field)\[0\].firstChild.data.strip())

</div>

 

<div>

             return
convert(x.getElementsByTagName(\"your\")\[0\].getElementsByTagName(field)\[0\].firstChild.data.strip())

</div>

 

 
