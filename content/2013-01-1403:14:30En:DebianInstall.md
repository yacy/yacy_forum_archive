En:DebianInstall
================

Date: 2013-01-14 03:14:30

added static IP configuration

← Nächstältere Version

Version vom 14. Januar 2013, 02:14 Uhr

Zeile 39:

Zeile 39:

 

<div>

When configured this way, the YaCy-internal auto-updater does not work.
An automatic update must be done with OS tools. i.e. with a crontab
command. An example for that is the following line, which you must write
into /etc/crontab

</div>

 

<div>

When configured this way, the YaCy-internal auto-updater does not work.
An automatic update must be done with OS tools. i.e. with a crontab
command. An example for that is the following line, which you must write
into /etc/crontab

</div>

 

<div>

  0 6 \* \* \* root apt-get update && apt-get -y \--force-yes install
yacy

</div>

 

<div>

  0 6 \* \* \* root apt-get update && apt-get -y \--force-yes install
yacy

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[After you configured YaCy, you may want also to set a \[\[En:StaticIP
\| static IP\]\] to get a unique IP to yout YaCy peer.]{.underline}

</div>

 

 

 

<div>

\[\[Category: Pages in English\]\]

</div>

 

<div>

\[\[Category: Pages in English\]\]

</div>
