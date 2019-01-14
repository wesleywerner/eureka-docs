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

    # Browse the docs at http://localhost:8000/
    $ sphinx-autobuild source/ build/

License
=======

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
