st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

Fork
----

This is my fork of the simple terminal. The changes at the config.h file were

1) Font changed to Inconsolata;
2) termname changed from "st-256colors" to "st";
2) Clipboard patch added;
3) Scrollback patch added;
5) No-bold-colors patch added since it is required by the Solarized patch;
5) Solarized patch added.

For completeness, the patch files used were added in the folder "patches".
