Traps
=====

Examples
--------

All trap examples can be played in :download:`traps.wad`

Monster Closet
--------------

Monsters are staged in a hidden room with a door disguised as a wall or other nondescript panel, which opens to surprise the player.

.. image:: monster_closet.png
    :target: /_images/monster_closet.png

* Create a hidden closet sector (A), add some monsters inside it.
* Create a closet door sector (B).
* Close the closet door so that it looks like a normal wall (C).
* Apply a fresh tag to the closet door sector (B).
* Add the trigger lines that will open the closet, and apply the same tag on them (D).
* Assign the linedef special **Type 109 W1 Open and stay fast** to the trigger lines (D).

Monster Platform
----------------

Monsters are staged on top a platform that lowers from the ceiling to surprise the player.

.. image:: monster_platform.png
    :target: /_images/monster_platform.png

* Add the platform sectors with some monsters in them (A).
* Raise the platform floors and ceilings (B) until flush with the surrouning ceiling.
* Select the platform sectors and apply a fresh tag (A).
* Insert vertices along a wall to make a 64 unit long line, for the switch (C).
* Set a switch texture (C).
* Apply the platform tags to the switch linedef (C).
* Set the switch linedef (C) type to **23 S1 Floor down LEF**.

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
