javascript gallery swipe-right rocket surgery
=============================================

Date: 2014-05-23 19:05:34

[![](http://www.jwz.org/images/ta43b.jpg)](http://www.dnalounge.com/gallery/dragnav.js)How
do I make page-swiping work properly in the [DNA Lounge photo
galleries](http://www.dnalounge.com/gallery/)? Go to any photo page and
swipe left or right on your phone. It goes to the next or previous
image, but it kinda sucks. I\'d like to de-suckify it.

My code is here:
[dragnav.js](http://www.dnalounge.com/gallery/dragnav.js).

What I\'d like:

-   Dragging animates the current page sliding out and the new page
    sliding in.

-   Presumably this would require pre-loading the HTML and images on
    both the next and previous pages, to get them in the cache early.

-   Dragging actually changes the page URL. (And changes it from
    \"`001.html`\" to \"`002.html`\", not to some bullshit like
    \"`index.html#002`\".)

-   Good answers come in the form of \"here\'s a Javascript snippet\"
    rather than in the form of \"here\'s a 30,000 line all-singing
    all-dancing mobile gallery application that does a ton of shit you
    don\'t care about.\"

Anyone?

[Previously](http://www.jwz.org/blog/2012/11/page-dragging-with-javascript/),
[previously](http://www.jwz.org/blog/2010/09/resizing-images-to-fit-the-window/),
[previously](http://www.jwz.org/blog/2014/03/a-hate-flower-that-blooms-all-year-also-space-egyptians/),
[previously](http://www.jwz.org/blog/2013/09/hoping-that-the-monsters-dont-do-what-monsters-are-always-going-to-do-because-if-they-didnt-do-those-things-theyd-be-called-dandelions-or-puppy-hugs/),
[previously](http://www.jwz.org/blog/2013/10/mobile-web-design-the-reign-of-morons-indeed/),
[previously](http://www.jwz.org/blog/2010/10/every-day-i-learn-something-new-and-stupid/).
