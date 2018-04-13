Traps
=====

Examples
--------

All trap examples can be played in :download:`traps.wad`

Monster Closet
--------------

Monsters are staged in a hidden room with a door disguised as a wall or other nondescript panel, which opens to surprise the player.

.. image:: monster_closet_layout.png

* Create a sector that will be your hidden closet:

.. image:: monster_closet_sector.png

* Add some monsters inside it.
* Join it with your room using a door-like sector:

.. image:: monster_closet_door.png

* Close the closet door so that it looks like a normal wall:

.. image:: monster_closet_3d.png

* Apply a fresh tag to the closet door sector.
* Add the trigger lines that will open the closet, and apply the same tag on them.
* Assign the linedef special *Type 109 W1 Open and stay fast* to the trigger line:

.. image:: monster_closet_trigger.png

Monster Platform
----------------

Monsters are staged atop a wall that lowers to surprise the player.

.. image:: monster_platform_3d.png

* Add the platform sectors with some monsters in them:

.. image:: monster_platform_sectors.png

* Raise the platform floors and ceilings:

.. image:: monster_platform_raised.png

* All the way to the top:

.. image:: monster_platform_raised_top.png

* Select the platform sectors and apply a fresh tag:

.. image:: monster_platform_tags.png

* Add a switch, apply the platform tags, set the type to **23 S1 Floor down LEF**:

.. image:: monster_platform_switch.png

Crushers
--------

The ceiling lowers, crushing the player.

.. note::

    You will need to unpeg the lower walls so they do not move up and down with the crushing ceiling.

Hole Trap
---------

A section of the floor drops out under the player,

Lock-In Trap
------------

Close the player in the room for a short period forcing them into combat

Teleport Ambush
---------------

Monsters stationed in a hidden room waken to the sound of gunfire, walk over a teleport trigger and summon themselves to a designated location.

Combat Teleporting
------------------

Use Type 126 WR Teleport /mon in a combat zone to warp monsters around the player while combat is taking place. This trap is used in Doom II map 10 to great effect with a Cyberdemon.

Nukage Surprise
---------------

A floor turns into radioactive waste, dealing damage to the player when walked on.

Exploding Barrels
-----------------