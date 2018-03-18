Eureka Manual
=============

This is a manual for the [Eureka Doom Editor](http://eureka-editor.sourceforge.net/)

Status
======

Work in progress

Building
========

[![Documentation Status](https://readthedocs.org/projects/eureka/badge/?version=latest)](http://eureka.readthedocs.io/en/latest/?badge=latest)

The docs are built with [Sphinx](http://www.sphinx-doc.org/en/master/#). You need Python installed, use `pip` to install Sphinx:

    $ pip install sphinx

For more installation options [see here](http://www.sphinx-doc.org/en/master/usage/installation.html).

To build:

    $ make html

To auto-build on change detection, and serve the site for development:

    $ sphinx-autobuild source/ build/

License
=======

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see http://www.gnu.org/licenses/.
