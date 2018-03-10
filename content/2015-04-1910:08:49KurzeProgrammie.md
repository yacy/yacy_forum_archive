Kurze Programmierer-Frage. Vielleicht kann das ja jemand \...
=============================================================

Date: 2015-04-19 10:08:49

Kurze Programmierer-Frage. Vielleicht kann das ja jemand von euch
autoritativ beantworten.

Ich habe mir vorhin folgendes überlegt. Nehmt euch mal sowas wie stdio.
Ausgaberoutinen. printf.

Da werden in Reihe lauter kleine Strings in einen Buffer geschoben. Im
Normalfall ist in dem Buffer ausreichend Platz für den String.

Mir geht es konkret gerade um libowfat, nicht libc, aber die Konzepte
sind ja die selben.

Mein Buffer-Interface hat ein buffer\_puts (nimmt einen const char\*)
und buffer\_put (nimmt const char\* und ein size\_t). buffer\_puts ruft
buffer\_put auf und übergibt strlen() von dem String als Länge.

In dem Fall, in dem man einen konstanten String ausgibt, kann man sich
das strlen mit einer gcc-Extension sparen. Das sieht dann in der Praxis
so aus:

    #define buffer_puts(b,s) (__builtin_constant_p(s) ? buffer_put(b,s,strlen(s)) : buffer_puts(b,s))

\_\_builtin\_constant\_p evaluiert zu 1, wenn s zur Compile-Zeit als
konstant bekannt ist. In dem Fall ist das strlen kostenlos, wenn ich es
in dem Makro mache. So wird dann

    buffer_puts(buffer_1,"foo\n");

zu

    buffer_put(buffer_1,"foo\n",4);

Soweit, so gut.

Die nächste Überlegung war: Wenn ich in buffer\_put nun memcpy von dem
Quell-Puffer in den Ziel-Puffer mache, dann ist in dem Ziel-Puffer
normalerweise noch genug Platz, und es macht auch nichts, wenn ich da
ein paar Bytes mehr schreibe (solange ich vorher geguckt habe, ob genug
Platz ist, versteht sich). Eigentlich kann ich da statt byteweise auch
gleich in 16-Byte-Vektoren kopieren. Auf aktuellem x86 kosten unalignete
Zugriffe nichts zusätzlich. Wenn da also jemand \"foo\\n\" schreiben
will, kann ich auch einfach 16 Bytes schreiben, von denen in den
vorderen \"foo\\n\" steht. Die entsprechende Buchhaltung in dem Buffer
muss ich natürlich mit der gewünschten Länge machen, nicht aufgerundet.

Aber dann dachte ich mir: OK, beim Schreiben ist das OK, wenn ich mehr
schreibe, das habe ich unter Kontrolle. Aber wie ist das beim Lesen? Ist
es denkbar, dass ein Programm mir den letzten String im
Read-Only-Datensegment übergibt, und wenn ich da einen ganzen Vektor
lese, dann renne ich über das Seitenende hinaus und crashe das Programm?

Für mein Dafürhalten sieht das gerade eher unwahrscheinlich aus. In
meinem Testprogramm kommen nach meinen Konstanten noch die ganzen
Konstanten der libc. Und dann sind hinter dem letzten String auch noch
mal ein paar Nullbytes Alignment vom Linker.

Meine Frage jetzt: Kennt jemand ein Szenario, in dem man nicht noch
(schlimmstenfalls) 15 weitere Bytes hinter dem Ende eines konstanten
Strings lesen kann? Wie ist das bei Windows? Wohlgemerkt reicht es
nicht, wenn das ein const char\* ist, damit das getriggert wird. Das
muss tatsächlich eine Stringkonstante sein.

**Update**: Valgrind hat keine Einwände.
