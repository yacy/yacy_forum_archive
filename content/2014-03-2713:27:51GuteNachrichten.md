Gute Nachrichten für Krypto-Hacker: GMP 6 ist draußen \...
==========================================================

Date: 2014-03-27 13:27:51

Gute Nachrichten für Krypto-Hacker: [GMP 6 ist
draußen](https://gmplib.org/gmp6.0.html) und implementiert erstmalig
\"side-channel silent\"-Versionen von den für RSA benötigten Primitiven.
OpenSSL hat eine eigene Implementation von Bignum-Funktionen und
profitiert daher nicht, aber einige anderen SSL-Libraries basieren ihre
Arithmetik auf GMP.

Wenn man es ernst meint, muss man natürlich auch seine symmetrischen
Cipher alle einmal anfassen, was sich teilweise massiv negativ auf die
Performance auswirkt, wenn man nicht z.B. AES per spezieller
AES-CPU-Instruktion macht.

Lustig an den Release-Notes ist auch unten die MISC-Kategorie, wo sie
die ganzen BSDs auflisten, auf denen das nicht oder kaputt kompiliert,
weil die Infrastruktur stinkt. Wer dachte, im Jahre 2014 haben wir
plattformübergreifend robuste und belastbare
Softwareentwicklungs-Infrastruktur am Start, der täuscht sich halt.
