
aDWM (attention deficit) Window Manager
=======================================
Forked from Luke Smith's build of dwm.

I just made some aesthetic changes, most NOTABLY, more noticable borders and the contrast of [SchemeNorm, SchemeSel]. I've always had a hard time trying to get the controls in my system because I didn't really know most of the time where the focus is. I was just tinkering around with the colors because I'm kinda getting sick of the default color suckless have provided, and so, I tried experimenting with gruvbox's colors (which are really pretty) and got the dark mode hard contrast and I think it was pretty nice and keeps me on focus ;).

That's just the cringe and bluepilled stuff that I have bloated in here. I wish I could add some colorful emojies so it'd be more prettier but I don't think it's possible.

Screenshot(s)
===========
![screenshot] [screenshot.jpg]

== Original README ==
dwm - dynamic window manager
============================
dwm is an extremely fast, small, and dynamic window manager for X.


Requirements
------------
In order to build dwm you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (dwm is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dwm (if
necessary as root):

    make clean install


Running dwm
-----------
Add the following line to your .xinitrc to start dwm using startx:

    exec dwm

In order to connect dwm to a specific display, make sure that
the DISPLAY environment variable is set correctly, e.g.:

    DISPLAY=foo.bar:1 exec dwm

(This will start dwm on display :1 of the host foo.bar.)

In order to display status info in the bar, you can do something
like this in your .xinitrc:

    while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
    do
    	sleep 1
    done &
    exec dwm


Configuration
-------------
The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.
