OpenGl multisampling performance
================================

Date: 2014-09-10 23:33:03

Dear Lazyweb,

If you turn on multisampling in xscreensaver on OSX, like this:

> ` defaults -currentHost write org.jwz.xscreensaver.Geodesic multiSample -bool true`

then one or two things happen. The first is, everything looks much
prettier because the polygon edges are anti-aliased. Yay. But the second
is, *sometimes*, the frame rate drops from 30fps to like 5fps, and CPU
utilization goes up to 95%. Boo.

I don\'t understand under what circumstances multisampling kills
performance. I assume it\'s exhausting some resource and falling back to
software rendering, though I don\'t know what that resource is or what
else is contending for it. Also, I haven\'t seen this happen on my
current machine. I last saw it on a Mac with a GeForce 8800 GS in it,
which is something like a 2008-vintage graphics card.

So\... I\'d like to turn on multisampling by default, except on machines
where that\'s likely to suck.

Perhaps the question I want to ask is, \"does this machine\'s video card
have gobs and gobs of RAM?\" Or maybe it\'s just, \"was this machine\'s
video card manufactured after 2013?\"

Do any of you know how to ask questions like that of an NSOpenGLContext,
or using some other MacOS API?
