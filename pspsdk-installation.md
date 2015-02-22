What does this do?
==================

This program will automatically build and install a compiler and other tools used in the creation of homebrew software for the Sony Playstation Portable handheld videogame system.

How do I use it?
==================

1. Set up your environment by installing the following software:

        autoconf, automake, bison, flex, gcc, g++/gcc-c++, libusb-dev, make, ncurses, patch, readline, subversion, texinfo, wget, mpc, gmp, libelf, mpfr, git

2. Set the PSPDEV and PATH environmental variables:

        export PSPDEV=/usr/local/pspdev
        export PATH=$PATH:$PSPDEV/bin

    The PSPDEV variable is the directory the toolchain will be installed to, change this if you wish. If possible the toolchain script will automatically add these variables to your systems login scripts, otherwise you will need to manually add these variables yourself.

3. Run the toolchain script:

        ./toolchain.sh

OSX
---

1. Install [`port`][MacPorts] or [`brew`][HomeBrew].
2. Install needed libraries: 

		sudo port install autoconf automake bison flex ncurses readline subversion texinfo wget mpfr

	or 

		sudo brew install autoconf automake bison flex ncurses readline subversion texinfo wget mpfr

 

3. Run `prepare-mac-os.sh`. This will auto-install rest of the dependencies
        
        sudo ./prepare-mac-os.sh

4. Build and install the toolchain and SDK.
        
        sudo ./toolchain-sudo.sh


Troubleshooting
===============

automake
--------
psp tool chain needs automake 1.9 version. Any other version won't work and error message can be a little bit misleading.


toolchain-sudo.sh
-----------------
If you're experiencing problems while running toolchain-sudo.sh break it down using 

		sudo ./toolchain-sudo.sh x

where `x` is replaced by number from 1 to 12 denoting part of buildscript (take a look at `/scripts` directory)


Building hello world
====================
Just follow steps from [PSP Programming Book](http://en.wikibooks.org/wiki/PSP_Programming)


