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

Your package manager might contain Eureka, albeit if outdated you can opt to build from source:

* Locate the latest version on `the release page <https://github.com/ioan-chera/eureka-editor/releases>`_
* Get and extract the source code
* Open a Terminal console.
* Install the build dependencies. On Debian-based distros the command may be:

::

    $ apt install build-essential cmake libopengl-dev libglx-dev libgl-dev libglu-dev libjpeg-dev libpng-dev libxpm-dev zlib1g-dev

If your Linux is running on X11 instead of Wayland, also add:

::

    $ apt install libpango1.0-dev libxft-dev

These are needed for proper font rendering and unicode support.
      
You may need to prepend these commands with ``sudo`` in case of "permission denied" errors.

The main user interface library, FLTK, will be downloaded during build, unless you add ``-DUSE_SYSTEM_FLTK=ON`` to the ``cmake`` command line. This will require a suitable ``libfltk`` installation, which may be ``libfltk-dev``, ``libfltk1.3-dev`` or ``libfltk1.4-dev``. Beware that if the maximum available system version of FLTK is 1.3, the application may behave incorrectly.

Now start making the binary. First, make sure you are in the extracted source code folder.

::

    $ cd path/to/eureka-source-folder

Substitute the actual extracted path here.

Now, since we use the ``cmake`` build system, a common pattern is to create a "build" subdirectory and enter it:

::

    $ mkdir build
    $ cd build

This will create a new ``build`` directory under the source code folder. Inside this folder, you will need to run the ``cmake`` tool. The recommended command line is (under Wayland you can omit the ``-DFLTK_GRAPHICS_CAIRO=ON`` option):

::

    $ cmake -DCMAKE_BUILD_TYPE=Release -DFLTK_GRAPHICS_CAIRO=ON ..

The ``-DCMAKE_BUILD_TYPE=Release`` ensures that what you produce will run at the best performance, and ``-DFLTK_GRAPHICS_CAIRO=ON`` (needed on X11) fixes some graphics issues with FLTK which may happen otherwise. It may not be required on every system. ``..`` means to tell ``cmake`` to load the information from the parent directory, which should be the one containing the source code, as extracted from GitHub.

If you get any errors of packages not found, try finding them via ``apt search`` followed by a key part of their name, then install them. If given multiple choices, pick the ones ending with ``-dev``.

If instead you opt to use a system-installed FLTK, do this instead:

::

    $ cmake -DUSE_SYSTEM_FLTK=ON ..

No Cairo specification is used in this case, because the system installed FLTK may have already been configured with it.

Now run ``make`` to perform the actual compilation:

::

    $ make

If it feels too slow, you can run something like ``make -j$(nproc)``, which parallelizes compilation to the number of CPU processors (``-j`` is the option to parallelize, and ``$(nproc)`` resolves to the number of processors). Again, as with ``cmake``, take note of any "missing header" errors which may be about missing dependencies, and install any of them as necessary.

If all went well, at this point you already have Eureka available. You can run the local build by going up one level and starting it, as this:

::

    $ ./eureka --install ..

The ``--install ..`` simply tells Eureka that the installation data -- typically the ``ugh`` configuration files and default key bindings -- are located in the parent directory. It does `not` install Eureka to the system.

After this, you can install Eureka to the system, so you can run it directly via the ``eureka`` terminal command from anywhere, and possibly also have an icon in the GUI desktop environment, using the following command:

::

    $ make install

You may need to prepend it with ``sudo`` if you get "permission denied" or "operation not permitted" errors.

.. warning::
    If you have installed an older Eureka version, and try to run a newer source-built version without installing it, the new one will still look for the configuration (``ugh``) files from the old installed app, which may be out of date. To prevent that, make sure to run this local build of Eureka using the ``--install`` command-line parameter (see `Invoking <invoking.html>`__ for the full list of command-line parameters).

.. note::
    Currently, Eureka won't detect its configuration files if installed to non-standard locations, i.e. others than ``/usr`` or ``/usr/local``, so you will need to invoke it with the ``--install`` command-line option explicitly in that case. This issue may be solved on next versions.

To uninstall Eureka later, you can run:

::

    $ make uninstall

This again may require ``sudo``. If it doesn't work, look inside an ``install_manifest.txt`` file that was generated during installation, and you will see the list of paths to manually delete (which again may require elevated privileges activateable with ``sudo``). If this file is missing, you can perform an installation instead (which should in effect do nothing), `then` retry uninstallation.
