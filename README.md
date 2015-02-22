PSP Developer Guide
==========
`PSP Developer Guide` is an attempt to gather remaing knowledge about PSP development in one place. PSP hype ended few years ago and now data/tutorials/sites are slowly dissapring from web. I hope that this repo won't die that easily :)

Basic information
-----------------
You need to install [psp-sdk](https://github.com/pspdev/pspsdk). I have created a little bit more detailed tutorial [here](pspsdk-installation.md) (although it is focused on OS X, I am sure that you can benefit from it on other platforms as well). 

I can recommend following book to create first app [PSP Programming Book](http://en.wikibooks.org/wiki/PSP_Programming)

Running
-------
You can use awesome [PPSSPP](http://www.ppsspp.org/) or of course real device (just copy `EBOOT.pbp` to `/PSP/GAME/YOUR_DIR/`).


Documentation
-------------
PSPSDK has code annotation that you can use to generate documenation. Just use `doxygen`. 

If you are too lazy it seems that there is a working copy:[pspsdk-doc](http://psp.jim.sh/pspsdk-doc/main.html)

Logging
-------
???

C++ support 
--------------
Don't forget to include `lstdc++` lib in your make file.

Examples
---------
[pspSnake](https://github.com/krzKaczor/psp-snake) - frame buffer, input, c++


Further reading
---------------
[platform overview](http://pspdev1.com/wp-content/uploads/2006/08/psp.pdf)

[bunch of tutorials](http://www.ghoti.nl/PSPtutorials.php)