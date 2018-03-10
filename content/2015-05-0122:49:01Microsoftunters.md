Microsoft unterstützt in Visual Studio 2015 Objective \...
==========================================================

Date: 2015-05-01 22:49:01

[Microsoft unterstützt in Visual Studio 2015 Objective
C](http://channel9.msdn.com/events/Build/2015/3-610). Seit einer Weile
gab es Gerüchte, dass Windows Phone einen Android-Emulator kriegen
sollte, um Android Apps ausführen zu können. Aber dann haben sie vor ein
paar Tagen völlig überraschend angekündigt, auch Ios-Apps unterstützen
zu wollen. Aber das ist nicht über einen Emulator, sondern man
kompiliert die dann neu. Da fragt man sich dann natürlich sofort: öh,
mit welchem ObjC-Compiler? Wo kommt das Runtime her? In obigem Video
sagen sie an, dass das Compiler-Backend das von Visual Studio ist. Das
ist schon mal echt überraschend, finde ich, denn so ein
Objective-C-Frontent zieht man sich nicht mal eben aus dem Hut.

Wo das Runtime herkommt, ist noch unklar.

In dem Video erzählen sie auch von neuen Security-Geschichten im
Compiler und, möglicherweise das spannenste daran, dass sie Coroutinen
in C/C++ implementiert haben, mit einem neuen Keyword namens yield.

Das ist ja mal echt beeindruckend viel Neuigkeiten, wenn man bedenkt,
dass die auch den Übergang zu C++11 / C++14 machen mussten in der Zeit,
und VS2015 auch Cross-Entwicklung für Android unterstützt. Wieviel Leute
da wohl im Compilerteam arbeiten?

Und: Wie lange es wohl dauert, bis gcc und clang auch yield
unterstützen? Im Moment fummelt man sich dort was mit Boost zurecht oder
so.

**Update**: OMG, die haben das Objective C-Frontend von clang geklaut
und ihren Codegenerator dahinter gepackt. \*Grusel\*
