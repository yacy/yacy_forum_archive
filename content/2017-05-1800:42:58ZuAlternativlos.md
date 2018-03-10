Zu Alternativlos 39 kamen eine Menge Leserbriefe rein. \...
===========================================================

Date: 2017-05-18 00:42:58

Zu Alternativlos 39 kamen eine Menge Leserbriefe rein. Erstens, zum
Update-Prozess von Windows:

> MS hat seit dem letzten W10 update delta updates, sie nennen es UUP\
> [blogs.windows.com](https://blogs.windows.com/windowsexperience/2017/03/02/an-update-on-our-unified-update-platform-uup/)\
> [blogs.windows.com](https://blogs.windows.com/windowsexperience/2016/11/03/introducing-unified-update-platform-uup/)

Ein zweiter Leserbrief beschreibt die Situation im Digital
Signage-Markt:

> wenn ihr schon so nett fragt kann ich ja mal ein paar Zeilen schreiben
> da ich beruflich so ein System entwickelt habe. 2010 brauchte ich
> einen neuen Job und wurde über einen ehemaligen Kollegen angesprochen
> ob ich nicht für eine Firma die Digital Signage macht ein Internet
> basiertes System neu entwickeln will.\
> Das VB6 System das die Firma bis dahin bai knapp 1000 Kunden am laufen
> hatte war in die Jahre gekommen und etwas das über einen Browser von
> überall her steuern war dringend erforderlich.
>
> Wie man sich sicher denken kann lief die alte Software auf Windows
> also sollte die neue Software auch darauf laufen - hier also schon mal
> der erste Grund warum Digital Signage auf Windows läuft - weil Version
> N-1 das getan hat. Hinzu kam das der technisch Verantwortliche (der
> die VB6 Version entwickelt hatte) darauf bestand verschiedene Teile
> der VB6 Version weiterzuverwenden (U.A. einen Laufschrift Generator
> der dank V-Sync seiner Meinung \"Broadcastqualität\" hatte).
>
> Den Kontrollserver durfte ich glücklicherweise als Linux System bauen.
> Der Windows-teil in in C\# geschrieben.
>
> Seit 2010 hat sich einiges getan auch hardwaremäßig und ich hatte
> versucht seit 2012 oder so die Client PCs durch etwas sinnvolleres wie
> einen Raspberry pi oder ein geeignetes Android System zu ersetzen.
> Leider war dafür nie Zeit bzw. die günstigere Hardware war nie ein
> genügendes Argument um die knapp 2 Monate in eine neue Player Software
> zu investieren. (Hier also Grund 2 - \"Warum es funktioniert doch\").
>
> 2013 wurde die kleine Firma durch eine Größere gekauft. Der Kollege
> der die VB6 Software geschrieben hatte verstarb plötzlich und die
> Firma wurde praktisch komplett aufgelöst und alle Mitarbeiter
> einschließlich des Geschäftsführers entlassen. Der einzige verblieben
> Mitarbeiter bin ich. Das Produkt für Digital Signage in Apotheken
> wurde einer anderen Größeren Unterfirma mit 150 Mitarbeitern
> zugeteilt.
>
> Meine neue Firma ist 100% Microsoft. Leute verwenden Windows 10 Handys
> hier. Ich denke das ist Grund 3 warum digital Signage auf Windows
> läuft - Die Funktionalität ist mittlerweile zu \"klein\" um das
> einzige Produkt einer Firma zu sein. Das heißt das diese
> Funktionalität als \"Zugabe\" zu anderer auf Windows basierter
> Software entwickelt wird. Und keine Firma die Windows Software baut
> verwendet dann Linux oder etwas anderes.
>
> Damit ist allerdings auch die Zukunft klar - der Kontrollserver wird
> auf ein Windows System umgestellt. Ich denke ich werde mich nach einen
> neuen Job umschauen.
>
> Die Frage \"Warum ist bei DS Systemen das Update ausgestellt\" hat
> auch ein paar Erklärungen- Digital Signage Systeme haben keine
> Benutzerinteraktion also fallen die häufigsten Infektionswege komplett
> weg - der Webbrowser und Email. Das macht es auch dank der Probleme in
> der jüngeren Vergangenheit mit durch WU installierte Popups (Windows
> 10 Nag und Office 356) einfach WU einfach auszuschalten weil wirklich
> die einzige Sicherheitslücke die das System überhaupt beeinträchtigen
> kann ein Remote Code Excecution Exploit ist - und die sind selten :/
>
> Bei uns war WU standardmäßig angeschaltet. Es gab allerdings immer
> wieder kleinere Probleme mit den entsprechenden Blasen und Popups die
> manchmal hoch kamen - die Windows 10 Nagscreens und die Office 356
> haben allerdings dafür gesorgt das Windows Update bei allen neuen PCs
> aus war.

Ein Dritter berichtet auch aus dem Signage-Markt:

> Ich sehe das Nichtupdaten bei Anzeigetafeln und ähnlichem Bullshit
> (mir fallen Spontan einige Industriesteuerungen ein, die zwar unter
> Debian laufen, aber im Prinzip das gleiche Problem haben): Gut
> gemeintes Firewalling.
>
> Diese Kisten erreichen alle anderen Kisten im LAN (müssen sie, denn
> ich muss die möglicherweise warten), aber nicht das Internet. Daraus
> folgt, dass die Dinger über die Existenz von Updates überhaupt nicht
> informiert sind! Jetzt reicht aber, dass eine blöde Kiste im LAN hängt
> und den Mist verbreitet und alle Kisten fallen um.
>
> Ein ähnliches Problem betrifft Rechner, die (aus Sicherheitsgründen
> oder weil sie einfach nicht gebraucht werden), garnicht oft am Netz
> sind.
>
> Ich bin im Übrigen ganz klar gegen Haftungsgeschichten, die haben
> nämlich schon den Schienenfahrzeugmarkt erfolgreich monopolisiert und
> zerstört.

Der [nächste
Beitrag](https://twitter.com/CptKrustenkaese/status/864860520855285760/photo/1)
ist kein Leserbrief aber passt gerade so schön...

Einen hab ich aber noch:

> Ich arbeite in einer Organisation (stolz auf ihr HighTech-Image) in
> der die IT, dass volle Program der Schlangenbeschwörung durchzieht,
> das ihr skizziert habt. Patches testen bevor man sie ausrollt,
> kumulieren. Schlangenöl auf allen Rechnern, Internet über Proxy,
> Microsoft blacklisten für \"pöse Websites\" (da ist dann auch schon
> mal das nameserver-config-interface von Schlund gesperrt), you name
> it...
>
> Es hat mich echt überrascht, dass ich bisher intern von einem
> wannacry-Befall nichts gehört habe.
>
> Ich selbst war lange IT-Leiter in einer grösseren Unterabteilung, mit
> viel spezial Krams für Geräteansteuerung. So wie ihr das beschrieben
> habt, nur noch gruseliger.
>
> Diese Lösungen sind oft in-house gestrickt von Leuten, die schon
> längst in Rente sind und die laufen eben. Und wenn man sie anfasst,
> fliegt es einem um die Ohren. Die stammen aus einer Zeit, wo es
> ausschliesslich darauf ankam, das etwas ans Laufen kam. programmiert
> haben das Leute, die ihre Gehversuche mit FORTRAN gemacht haben.
> Irgendwann haben sie sich C oder gar C++ beigebogen, aber immer noch
> Spaghetticode gemacht.
>
> Wenn du das anfassen willst, musst du es von Grund auf neu machen.
> Also gehst du zu deinem Management und versuchst, ein Budget zu
> bekommen. Wenn du Glück hast, bist du in ein paar Jahren!!! so weit,
> dass du deine Kisten mal upgraden kannst. Meist kriegst du aber kein
> Budget. Und für Security gibt es ja Schlangenöl.
>
> Wer entscheidet in Organisationen über die Bugjets? Das sind Leute,
> die sich für sehr wichtig halten und die fest daran glauben, was immer
> zu entscheiden ist, besser entscheiden zu können, als so ein Techie
> mit seinem schmalspurigen Blick auf die Welt. Das gilt für
> Produktionsanlagen und gilt erst recht für IT, denn der Manager hat ja
> daheim selbst einen PC und daher kennt er sich in IT besonders gut
> aus. Welche Erfahrungen haben diese Typen gemacht? Wenn man updates
> einspielt, geht danach irgentetwas nicht mehr. Das legt eine
> Teilaufgabe lahm, kostet Zeit und ist ärgerlich. Updates verändern die
> Applikation, so dass irgendetwas liebgewonnenes nun nicht mehr oder
> anders geht. Firmen nutzen Updates, um den Nutzer zu entmachten (die
> Digikam erkennt plötzlich den Akku aus dem Zubehör und spielt nur nach
> mit Originalakkus. Der Drucker verlangt nach HP-Patronen.) Kurzum, in
> ihrer Welt sind Updates von übel. Und das Internet war ehrlich gesagt
> bis dato nicht wirklich so gefährlich, oder? Mein damaliger Boss hatte
> nie einen Virus. Er war immerhin clever genug, nicht auf jeden Scheiss
> zu klicken. Und Backups hat er auch. Diese persönliche Erfahrung
> bestimmt weitesgehend seinen Managementstil. Also kriegst du kein
> Budjet, denn an anderen Stellen in der Bude brennt es viel dringender.
> (Z.B. braucht man Juristen, damit einem nix angeflickt wird oder so
> ..... jedenfalls keine Scheiss-Updates.)
>
> Nun komme ich zu dem entscheidenden Punkt: Ihr habt das T-shirt mit
> der Aufschrift \"told you so\" erwähnt. Wenn du als kompetenter
> Manager im IT-Bereich auf Risiken hinweist, ist das so lang o.k., wie
> du nach einiger Quälerei überzeugen kannst und das Budjet zur
> Umsetzung einer Maßnahme bekommst. Es ist unerquicklich, wenn du dich
> nicht durchsetzen kannst und du mit dem Risiko weiter leben mußt, weil
> dir per Order die Hände gebunden sind. Am schlimmsten ist aber, wenn
> du recht behälst. Vermutlich kannst du, wenn die Katastrophe eintritt
> sogar noch einen \"cover-my-ass-letter\" aus denm guten alten
> Leitzordner ziehen. Das machst du einmal, vielleicht zweimal. Sowas
> vetragen Manager gar nicht. Ich bin kein IT-Leiter mehr. Zum Glück war
> für mich das Arbeitsrecht noch so hart, dass ich eine Weile gemütlich
> auf dem Abstellgleis verbringen durfte und in ein paar Monaten in
> Rente gehen werde.
>
> Was wir verbreitet in allen Industrien haben, ist eine
> Managementkrise. Es ist nicht wirklich wichtig für die Zukunft zu
> denken. Wichtig ist, die Dinge so zu verwalten, dass man nicht
> persönlich zur Rechenschaft gezogen wird. Das was Gunther Dueck so
> treffend die anonymisierte Verantwortungslosigkeit nennt. Diese Art
> von Entscheidungkriterien betreffen auch die Securityfrage. Aber das
> war bisher eine winzige Baustelle im Vergleich zu anderen Ecken, wo
> mit dem Feuer gespielt wird.
>
> Zurück zu wannacry. Das einzig wirklich neue ist die Erkenntnis, dass
> einem so ein Angriff potentiell so abschiessen könnte, dass man nicht
> mehr auf die Hufe kommt. Da ist er in der öffentlichen Warnehmung der
> erste Fall. (Falls er überhaupt so wargenommen werden wird. Was sind
> schon ein paar Krankenhäuser!)
