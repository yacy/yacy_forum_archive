Endlich verbreitet auch mal ein Einsender Hoffnung \...
=======================================================

Date: 2018-01-08 19:57:51

Endlich verbreitet auch mal ein Einsender Hoffnung bezüglich Meltdown:

> Meltdown scheint ja am Gefährlichsten zu sein, da es Kernelmemory
> dumpen und auf andere Prozesse zugreifen kann, und ist sogar mit
> eigenem Logo am start. Es hat allerdings eine Einschränkung, die
> derzeit irgendwie keiner auf dem Schirm hat und die meiner Ansicht
> nach im Meltdown-Paper mindestens unvollständig oder gar falsch steht.
> Dort steht man könnte \"simple\" (über 0xffff8800xxx) den gesamten RAM
> auslesen:
>
> <https://meltdownattack.com/meltdown.pdf>
>
> Seite 11: \"On such systems, an attacker can use Meltdown to dump the
> entire physical memory, simply by reading from virtual addresses
> starting at 0xffff 8800 0000 0000.\"
>
> Alle existierenden PoCs, sowie meine Tests und auch Google kommen
> allerdings zu einem anderen Ergebnis:
>
> <https://googleprojectzero.blogspot.de/2018/01/reading-privileged-memory-with-side.html>
>
> \"PoC for variant 3 that, when running with normal user privileges,
> can read kernel memory on the Intel Haswell Xeon CPU under some
> precondition. We believe that this precondition is that the targeted
> kernel memory is present in the L1D cache.\"
>
> Man kann das - offensichtlich - nur ausnutzen, wenn man das
> auszulesende \"Geheimnis\" im Speicher bereits im L1 Cache der
> gleichen CPU hat, was kein triviales Problem ist, wenn man es selbst
> nicht lesen darf und auch (von mir getestet) Befehle wie prefetch oder
> simpler Zugriff über MOVen vom unberechtigten Prozess kein L1 Caching
> bewirken.
>
> Schön kann man diese Anhängigkeit an allen so funktionierenden und
> verfügbaren Meltdown-Code sehen, die im Kernel \"linux\_proc\_banner\"
> ausgeben: Das geht erst, wenn man \"/proc/version\" öfters ausliest,
> und es damit in den L1 Cache gelangt:
>
> <https://github.com/paboldin/meltdown-exploit>
>
>         fd = open("/proc/version", O_RDONLY);
>     …
>             ret = pread(fd, buf, sizeof(buf), 0);
>             if (ret < 0) {
>                 perror("pread");
>                 break;
>             }
>
> <https://github.com/Frichetten/meltdown-poc>
>
>      +      int fd = open("/proc/version", O_RDONLY);
>      +      int ret = 0;
>      +      char thing[256];
>      +      ret = pread(fd, thing, sizeof(thing), 0);
>
> \"Added the ability to dump the linux\_proc\_banner\"
>
> Also wer KVM betreibt, der wird von Spectre 2 nicht so begeistert
> sein. Browserhersteller finden Spectre 1 und 2 nicht so toll. Auch ist
> Meltdown natürlich nicht schön, allerdings doch auch nicht so krass
> wie bisher geschrieben: Memoryauslesen geht nur wesentlich
> eingeschränkter als bislang behauptet.
>
> ... Darum gibts wohl auch keine wirklichen Exploits?
>
> Es ist mir übrigends bislang allgemein auch noch nicht gelungen auch
> nur ein Byte über 0xffff bb00... den Speicher eines anderen Prozesses
> auszulesen, auch über verschiedenste Prozessoren hinweg
> (i3,i5,i7,Xeon,...). Nicht eines! Und ja, ich habe KASLR
> berücksichtigt. Selbst ein mikriges Testprogramm, dass mit Malloc auf
> dem heap etwas ablegt und es ständig per printf ausgibt, ist nicht
> auslesbar - mich würde interessieren ob das mit dem angeblichen 0xffff
> bb00, das sich ja mit der Kerneldoku deckt, allgemein falsch ist - so
> wie es der Googlepost ja nahelegt - oder was da noch falsch sein
> könnte...

Sehr erfreulich! Vielleicht geht die Welt ja doch noch nicht unter.
