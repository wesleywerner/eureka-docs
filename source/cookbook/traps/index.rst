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

The ceiling lowers to crush the player.

.. image:: crusher.png
    :target: /_images/crusher.png

* Assign a fresh tag to the sector that will do the crushing (A).
* Create a linedef that will act as the walk-over trigger (B).
* Assign the same tag to the trigger linedef (B).
* Set the trigger linedef (B) **Type 6 W1 Crusher /fast**

.. note::

    You will need to **lower unpeg** the room sector walls (C) if you do not want the walls to move up and down with the crushing ceiling.

.. warning::

    Fast crushers do less damage and the player may even survive one round of crushing. Slow crushers take their time, dealing a lot of damage and ensures player death.

Drop Trap
---------

The floor drops out unexpectly from beneath the player into a room with monsters.

.. image:: drop_trap.png
    :target: /_images/drop_trap.png

* Add the sector that will drop out beneath the player (A).
* Tag the sector (A).
* Add the hidden room the player will drop into, lower it's floor (B).
* Insert vertices on a wall to create a switch (C).
* Set the tag of the switch linedef (C) to match the drop sector (A).
* Set the switch linedef **Type 123 SR Lift Lower /fast** (C).


Lock-In Trap
------------

Lock all the exits in a room, forcing the player into close combat for a short time.

.. image:: lock-in_trap.png
    :target: /_images/lock-in_trap.png

* Create the open door sector (A) and assign a fresh tag to it.
* Add the linedef that will trigger the door to close (B).
* Set the linedef **Type 16 W1 Close for 30s**

.. note::
    If you want to close multiple doors in the room, give them all the same tag.

Teleport Ambush
---------------

Monsters stationed in a hidden room wake up to the sound of gunfire, walk over a teleport trigger and summon themselves to the designated location.

.. image:: teleport_ambush.png
    :target: /_images/teleport_ambush.png

* Apply a fresh tag to the sector where the monsters will teleport into (A).
* Insert the **Teleport exit** thing (type 14, under the "Player" category called `TFOG`) in the sector (A).
* Create a hidden room where the monsters are stationed (D).
* Connect the main sector (A) with the hidden room (D) via a sound pipe (B). This allows the sound of gunfire to reach the hidden room, alerting the monsters.
* Insert a teleport trigger linedef in the hidden room (C), assign the same tag as the exit sector (A), and set the **Type 97 WR Teleport**.

.. note::

    Use the **Sound Sector Rendering** mode (under the View menu), and enter **sector edit mode** in the 2D view to see how sound travels in your map.

Combat Teleporting
------------------

Use Type 126 WR Teleport /mon in a combat zone to warp monsters around the player while combat is taking place. This trap is used in Doom II map 10 to great effect with a Cyberdemon.

Nukage Surprise
---------------

A floor turns into radioactive waste, dealing damage to the player when walked on.

Exploding Barrels
-----------------
