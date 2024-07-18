Eureka Manual
=============

This is a manual for the [Eureka Doom Editor](http://eureka-editor.sourceforge.net/).

Status
======

Stable

[![Documentation Status](https://readthedocs.org/projects/eureka/badge/?version=latest)](http://eureka.readthedocs.io/en/latest/?badge=latest)

Building
========

The docs are built with [Sphinx](http://www.sphinx-doc.org/en/master/#). Consult the Sphinx documentation for installation instructions.

```
# Provision a virtual environment
python -m venv .venv

# Activate the environment (Windows)
.venv\Scripts\activate.bat

# or Activate the environment (*nix)
source .venv/scripts/activate

# Install Sphinx
pip install sphinx
```

To build the documentation:

```
# Activate the virtual environment (if not already) then
make html
```

License
=======

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
