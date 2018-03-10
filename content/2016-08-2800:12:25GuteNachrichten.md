Gute Nachrichten! Es ist mal wieder Zeit für ein OpenSSL-Update. \...
=====================================================================

Date: 2016-08-28 00:12:25

Gute Nachrichten! [Es ist mal wieder Zeit für ein
OpenSSL-Update](https://www.openssl.org/blog/blog/2016/08/24/sweet32/).
Nicht nur OpenSSL, das Problem ist gar kein spezifisches in OpenSSL,
sondern dass 64-bit Block Cipher inzwischen realistisch per Birthday
Attack angreifbar sind. Bei TLS betrifft das Cipher mit 3DES, bei VPNs
betrifft das Blowfish. OpenSSL \"\"löst\" das, indem sie 3DES von HIGH
nach MEDIUM schieben in 1.0x und in 1.1 fliegt es ganz raus. [Details zu
dem Angriff](https://sweet32.info/).
