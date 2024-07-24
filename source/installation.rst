Installation
============

Also see the official `Eureka command line parameters <https://eureka-editor.sourceforge.net/Docs_Invoking.html>`_ page.

Requirements
------------

A IWAD file, or "Internal WAD", contains the default maps, textures, sounds and other auxiliary data. You can use the `DOOM.WAD` or `DOOM2.WAD` files if you own those.

Alternatively you can download the `Freedoom <http://freedoom.github.io/>`_ WADS, Freedoom is liberally licensed under the BSD license and provides free levels, artwork, sound effects and music compatible with any classic Doom source port. Download and extract Freedoom to an accessible location of your choice. If you are a GNU / Linux user you may extract the Freedoom WADS into ``~/.eureka/iwads/`` where they are automatically detected for your convenience.

.. note::

    A PWAD file, or "Patch WAD", provides additional levels and other resources that replace those in the IWAD. When making levels in Eureka we will be working with PWADs - any mention of a WAD file implies the PWAD unless otherwise noted.

Doom Engine
^^^^^^^^^^^

You will need a Doom source port to play-test your maps. Here are a couple of options you can browse:

* `Chocolate Doom <https://www.chocolate-doom.org>`_ - accurately reproduces the experience of Doom as it was played in the 1990s. A safe option for testing your maps.
* `PrBoom <http://prboom.sourceforge.net/>`_ - an advanced engine with fine-grained control over options controlling compatibility levels. This port is the standard for recording and playing of demos.
* `Crispy Doom <https://fabiangreffrath.github.io/crispy-doom>`_ - a minimalist engine with few extra features.
* `GZDoom <https://gzdoom.drdteam.org/>`_ - an advanced and moddable engine with many features, including newer and non-standard features. You should not base your map's compatibility off this port alone.

Windows
-------

To get the latest Eureka for Windows, go to the `Eureka release page <https://github.com/ioan-chera/eureka-editor/releases>`_ and choose the latest version. Extract the zip somewhere memorable and run `eureka.exe`.

macOS
-----

Similar to Windows, download the DMG archive from the release page, open it in Finder, and when presented with the folder window, drag `Eureka Doom Editor` into the `Applications` linked folder. You can choose the DMG archive for AppleSilicon (M1/M2 ARM) modern processors, or the one for older Intel processors, depending on your Mac.

GNU / Linux
-----------

Your package manager might contain Eureka, albeit if outdated you can opt to build from source.

* Locate the latest version on `the release page <https://github.com/ioan-chera/eureka-editor/releases>`_
* Get and extract the source code
* Install the build dependencies:

::

    $ sudo apt-get install \
    build-essential \
    libfltk1.3-dev \
    libxft-dev \
    libxinerama-dev \
    libfontconfig1-dev \
    libjpeg-dev \
    libpng12-dev \
    zlib1g-dev \
    xdg-utils

* make the binary

::

    $ cd eureka*
    $ mkdir build
    $ cd build
    $ cmake ..
    $ make

* install Eureka

::

    $ sudo make install

.. note::

    See file INSTALL.txt included with the Eureka source for detailed build instructions.
