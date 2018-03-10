Heartbleed scheint die Szene wachgerüttelt zu haben. \...
=========================================================

Date: 2014-04-13 22:12:07

Heartbleed scheint die Szene wachgerüttelt zu haben. [Akamai hat ein
paar Patches
veröffentlicht](http://thread.gmane.org/gmane.comp.encryption.openssl.user/51243?resub=1),
um die Serverschlüssel zwischen Guard-Pages zu speichern, damit die nie
als Teil von sowas wie Heartbleed rausleaken können. Sie sagen, sie
fahren damit seit 10 Jahren ihre Server.

[OpenBSD hat einen Audit angestoßen und der zeitigt erste
Ergebnisse](http://ftp.openbsd.org/pub/OpenBSD/patches/5.4/common/008_openssl.patch).

Und nicht zuletzt: [Coverity, einer der bekannteren
Code-Scanner](http://blog.regehr.org/archives/1128), der hat Heartbleed
nicht erkannt. Der Firma ist das einigermaßen peinlich, daher haben sie
jetzt nach Heuristiken gesucht, um sowas doch zu finden, und dabei
hatten sie eine relativ smarte Idee: Endianness-Konvertierung markiert
bei denen jetzt Variablen als vergiftet. So gehen Code-Auditoren wie ich
auch vor.

Ich habe die Tage erfreut festgestellt, dass PolarSSL auch ECDSA kann
inzwischen, EDH eh schon, und jetzt auch GCM. Damit haben sie soweit
alle wichtigen Features. Auf Client-Seite ist die
Zertifikats-Validierung wohl noch nicht so toll, ich verlinkte neulich
die Frankencert-Tabelle. Aber das ist ja serverseitig wurscht, außer man
will Client Certs haben, was so gut wie niemand tut. Das ist neben
OpenSSL die andere unterstützte SSL-Engine in gatling und von der
Codequalität her macht sie einen ganz guten Eindruck. Viel kleiner und
ordentlicher und weniger Makrohölle als OpenSSL. Klein genug, dass eine
Einzelperson davon realistisch einen Komplett-Audit machen könnte.
