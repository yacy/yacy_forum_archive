En:DebianInstall
================

Date: 2016-05-08 09:57:34

[Managing YaCy: ]{.autocomment} added use of systemctl to control
automatic startup

← Nächstältere Version

Version vom 8. Mai 2016, 07:57 Uhr

Zeile 43:

Zeile 43:

 

<div>

  /etc/init.d/yacy start

</div>

 

<div>

  /etc/init.d/yacy start

</div>

 

<div>

  /etc/init.d/yacy restart

</div>

 

<div>

  /etc/init.d/yacy restart

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[You can use systemctl (run as root) to enable or disable YaCy automatic
startup at boot.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[Enable automatic startup :]{.underline}

</div>

 

\+

<div>

[systemctl enable yacy]{.underline}

</div>

 

\+

<div>

[Disable automatic startup :]{.underline}

</div>

 

\+

<div>

[systemctl disable yacy]{.underline}

</div>

 

 

 

<div>

The YaCy web server runs on port 8090 by default. The administration
pages are at

</div>

 

<div>

The YaCy web server runs on port 8090 by default. The administration
pages are at

</div>
