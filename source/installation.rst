Installation
============

Windows
-------

Locate the latest version on `the download page <https://sourceforge.net/projects/eureka-editor/files/Eureka/>`_ and grab `eureka-*-win.zip`.

GNU / Linux
-----------

* Locate the latest version on `the download page <https://sourceforge.net/projects/eureka-editor/files/Eureka/>`_
* Get `eureka-*-source.tar.gz`
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

    $ make

* install Eureka

::

    $ sudo make install

*See file INSTALL.txt included with the Eureka source for detailed build instructions.*


Doom Engine
-----------

To test our maps we need a Doom engine, we will use the PrBoom engine as it is multi-platform. Go ahead and `install PrBoom <http://prboom.sourceforge.net/>`_ or via your package manager.

IWAD Configuration
------------------

This guide will use the `Freedoom <http://freedoom.github.io/>`_ IWAD, download and extract Freedoom to an accessible location of your choice. If you are a GNU / Linux user you may extract the Freedoom WADS into ``~/.eureka/iwads/`` for convenience.
