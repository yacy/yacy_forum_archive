Aktuelles Highlight aus dem OpenSSL-Cleanup von OpenBSD:Do \...
===============================================================

Date: 2014-04-17 18:56:17

[Aktuelles Highlight aus dem OpenSSL-Cleanup von
OpenBSD](http://marc.info/?l=openbsd-cvs&m=139773689013690&w=2):

    Do not feed RSA private key information to the random subsystem as
    entropy.  It might be fed to a pluggable random subsystem....What were they thinking?!

Äh ja, die Frage stellt sich. Ich stelle mir das ungefähr so vor:

> Hey, Cheffe, wir brauchen hier mal Entropie für den
> Zufallszahlengenerator!
>
> Was sagst du? Krypto-Schlüssel haben eine hohe Entropie?
>
> OK, Cheffe, knorke, wird gemacht!

m(
