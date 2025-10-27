Installation
============

Also see the official `Eureka command line parameters <invoking.html>`_ page.

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
* `Eternity Engine <https://eternity.youfailit.net/wiki/Main_Page>`_ - another advanced and moddable engine, designed in particular for backwards compatibility with less advanced engines while still adding new features.

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
* Install the build dependencies. On Debian-based distros the command may be ``sudo apt-get install build-essential``. You will also need to install the following libraries: X11, JPEG, PNG and ZLIB.
  The main user interface library, FLTK, will be downloaded during build, unless you add ``-DUSE_SYSTEM_FLTK=ON`` to the ``cmake`` command line.

* Make the binary:

::

    $ cd eureka*
    $ mkdir build
    $ cd build
    $ cmake -DCMAKE_BUILD_TYPE=Release ..
    $ make

* Install Eureka:

::

    $ sudo make install

.. warning::
    If you have an older Eureka version installed on the system, and try to run a more modern local source-built version of it, it will look for the installed configuration (`ugh`) files which came with the older version, and possibly result in user interface inconsistencies or errors. To prevent that, make sure to run this local build of Eureka using the `--install` command-line parameter (see [invoking] for the full list of parameters):

::

    $ build/eureka --install .

.. note::
    See file INSTALL.txt included with the Eureka source for more build details.

* To uninstall Eureka later, you can run:

::

    $ sudo make uninstall

or delete all files listed in the ``install_manifest.txt`` file produced during installation.
