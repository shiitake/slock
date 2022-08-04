slock - simple screen locker
============================
simple screen locker utility for X.


### Fork Details ###

Patches applied: 
* [Capscolor](https://tools.suckless.org/slock/patches/capscolor) - indicates whether or not capslock is on. 
* [Message](https://tools.suckless.org/slock/patches/message) - Lets you add message to the lock screen 
* [Xresources](https://tools.suckless.org/slock/patches/xresources) - Lets you specify colors through your .Xresources file 
* [Quick Cancel](https://tools.suckless.org/slock/patches/quickcancel) - Cancel slock by moving the mouse within a certain time-period. 
* [background-image](https://tools.suckless.org/slock/patches/background-image) - Let's you specify background image in config.h 

**Notes** 
You can customize the location of the background image file in `config.def.h`. The default location is `/usr/local/share/wallpaper/screen-lock.png`. This image file will need to be accessible to whichever user is specified in the config file. The default user is `nobody`. 






Requirements
------------
In order to build slock you need the Xlib header files.  For the applied patches you will also need `libimlib2-dev` (for Background Image patch) and `libxinerama-dev` (for messaging). 


Installation
------------
Edit config.mk to match your local setup (slock is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install slock
(if necessary as root):

    make clean install


Running slock
-------------
Simply invoke the 'slock' command. To get out of it, enter your password.

