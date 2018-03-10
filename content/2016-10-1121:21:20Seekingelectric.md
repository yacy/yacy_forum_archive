Seeking electric motor for serious relationship
===============================================

Date: 2016-10-11 21:21:20

![](https://www.jwz.org/curtain/100-thumb.jpg)Lazyweb,

I need a better motor for my [curtain
automation](https://www.jwz.org/curtain/). I\'ve tried several models,
and they all only last two or three months before they strip their
internal gears. So my current procedure is, \"buy a new motor every two
months.\" This is not a good system.

I figured the motors would just stall out before stripping gears. They
are straining, but never reach the point where they actually stop
turning. But no, eventually something cracks.

I\'m driving the motors with with [this
board](https://www.adafruit.com/products/1438), which is 12vdc and has a
1.2a max stall current, so I\'ve tried these motors, and stripped the
internal metal gears on all of them, multiple times:

-   [227:1 1.1A](https://www.pololu.com/product/3257)
-   [378:1 1.1A](https://www.pololu.com/product/3258)
-   [227:1 2.1A](https://www.pololu.com/product/3233) (which is
    technically out of spec for the driver, but worked-ish)

I\'m kind of puzzled by this, because except for the 227:1 1.1A, they
are not stalling out! They strain a bit at the end, but they keep
turning. I expected that the failure mode I would be repeatedly
experiencing would be that the motor is fine and the driver board melts.
But somehow, even without the motor ever getting stuck, it\'s just
shattering internally. (Applying power directly results in the shaft not
rotating at all, or rotating only partially then getting stuck, so it\'s
definitely that the gearbox has committed internal suicide.)

I need to find a quiet, fast motor with like, 350+ oz-in torque.
Bidirectional, constant speed. And if it has more than a 1.1A stall, or
if it needs more than 12vdc, I need to find a driver board to run it
with. I don\'t even really know where to look. You\'d think lots of
people would want to move heavy things with a small box.

Suggestions?
