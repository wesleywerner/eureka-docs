Running Eureka
==============

You can run Eureka a number of ways: from double clicking its binary after downloading and unpacking (the Windows and macOS packages), from the desktop menu (when installed e.g. from the Debian repository), or from the command line in a terminal emulator.

Note that Eureka needs a game IWAD in order to run.  When it cannot find one, then the "Manage Wads" dialog will open up and you can use the "Find" button to locate one. If you do not own any of the games which Eureka supports, there is always the project "FreeDoom" which is completely free.

The rest of this page describes running Eureka from the command line.

----

Option Syntax
-------------

Option names begin with either one or two dashes.  Short options consist of a single letter after a single dash, like ``-f`` and ``-w``, whereas long options are a whole word following one or two dashes, such as ``--file`` and ``--warp``.  Long options are shown on this page with two dashes, but a single dash is supported too, because that syntax was accepted by the original DOOM engine and various source ports.

Some options accept a parameter after them.  There *must* be a space between the option name and the parameter, even for short options, and equal signs *cannot* be used.  A few of the options accept multiple parameters, and each parameter must be separated by spaces too.

When the first thing on the command line is not an option, Eureka treats it as the filename of a pwad to edit.  Multiple files can be specified this way.

Examples of valid options:

    ``-w 1``

    ``-warp 2``

    ``--warp 3``

Examples of **invalid** options:

    ``-w``  *missing the parameter*

    ``-w2``  *no space between option and parameter*

    ``-w=3``  *equal signs cannot be used*

----

General Options
---------------

**-f  -\-file <filename>....**

    The wad file(s) to edit.  When more than one filename is given, the first one is opened for editing, and the others can be accessed from the "Given Files" sub-menu(in the File menu.

**-w  -\-warp <map>**

    Which level to edit.  This can be the full map name, such as "MAP12" or "E3M4", but can also be a single number like "12" or "34", and for Ultimate DOOM and Heretic a pair of numbers (episode + map) is supported too.

**-i  -\-iwad <filename>**

    The name of the game IWAD file.  This specifies what game you are editing for, e.g. "doom.wad" will mean the map is for Ultimate DOOM, whereas "heretic.wad" means we are editing for the game Heretic.

**-m  -\-merge <filename>....**

    Resource file(s) to load.  These can be wad files containing textures, flats, sprites (etc), but can also be Eureka definitions files (with the ``.ugh`` extension).

**-p  -\-port <name>**

    Name of the port (engine) being used.  The default port is "vanilla", which refers to the original DOOM EXE (or to Chocolate-Doom), but some other supported ports are "boom", "mbf", "edge", "odamex", "legacy" and "zdoom".

**-h  -\-help**

    Show a usage summary.

**-v  -\-version**

    Show the version string.

**-q  -\-quiet**

    Inhibits messages to the terminal.  NOTE: has no effect on beeping!

**-d  -\-debug**

    Enable extra debugging messages.

----

Configuration Options
---------------------

The following options control how Eureka finds some important files and directories.   They are not particular useful *per se*, but may be needed for special circumstances.

**-\-install <dir>**

    The installation directory where game definition files, default key bindings, and a few other important files are located.  Specifying "." for the install directory is useful when compiling and testing Eureka.

**-\-home <dir>**

    The home directory where user settings, wad backups, and a few other files are stored.  Under Linux and other Unixes, this will be the ``.config/eureka`` folder in the user's ``$HOME`` directory.

**-\-log <file>**

    The file where all log messages are written.  Defaults to ``logs.txt`` in the home directory.

**-\-config <file>**

    The config file which stores all the user's preferences (except for key bindings).  This file is loaded when Eureka starts up, and is saved whenever the user uses the Preferences dialog.  Defaults to ``config.cfg`` in the home directory.

----

Environment Variables
---------------------

The following environment vars are recognized by Eureka:

**DOOMWADDIR**

    If set, contains a single directory name where Eureka  will look for IWADs.

**DOOMWADPATH**

    If set, contains a colon-separated list of directories where Eureka will look for IWADs.
