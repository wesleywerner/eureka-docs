Building Basics
===============

These building basics focus on level geometry only. There is no logic or game triggers here.

Vertices
--------

Vertices are the joins between Linedefs and the corners between walls.

* Press :kbd:`v` in the 2D view to enter Vertices edit mode
* :kbd:`LMB` while hovering over a Linedef inserts a single vertice at the cursor position
* :kbd:`RMB` inserts a vertice in **line drawing** mode, keep adding vertices with :kbd:`RMB` until you close the polygon

.. image:: /images/basics/vertices.png

Linedefs
--------

Linedefs define the areas in a map. Every linedef is between two vertices. Linedefs divide the map into sectors, and thet are also used to trigger actions.

Press :kbd:`l` in the 2D view to enter Linedef edit mode.

.. image:: /images/basics/linedefs.png

A linedef also has a front and a back. You can tell the front of a Linedef by the direction of the protruding pin in the middle of the Linedef.

.. image:: /images/basics/linedef-front.png

*this linedef front is facing down*


Sectors
-------

A sector is an area defined by multiple Linedefs.

Press :kbd:`s` in the 2D view to enter Sector edit mode.

.. image:: /images/basics/sectors.png

Things
------

Things represent players, monsters, pick-ups, obstacles, decorations, player start positions and teleport landing sites.

Press :kbd:`t` in the 2D view to enter Things edit mode.

.. image:: /images/basics/things.png

Multiple Selections
-------------------

While in the 2D view, you can select Vertices, Linedefs, Sectors and Things by:

* Clicking an item to select/unselect it
* Drag-select multiple items to include/exclude them in the selection
* Hold :kbd:`shift` to prevent moving things around when making a selection

Switching between Vertices, Linedefs and Sectors will preserve any selections as much as possible.

Deselecting
-----------

Press :kbd:`\`` (back quote) in the 2D view to deselect everything.


Transformations
---------------

You can scale and rotate selected Sectors, Linedefs and Vertices.

Scaling
^^^^^^^

Click on :kbd:`Edit -> Scale Objects` or press :kbd:`F3` to show the scale dialog.

.. image:: /images/basics/scale-selection.png

*Four inner most vertices are selected*

.. image:: /images/basics/scale-dialog.png

*Scaling the vertices by 50% on the x-axiz*

.. image:: /images/basics/scale-result.png

Rotating
^^^^^^^^

Click on :kbd:`Edit -> Rotate Object` or press :kbd:`F4` to show the rotate dialog.

.. image:: /images/basics/scale-selection.png

*Four inner most vertices are selected*

.. image:: /images/basics/rotate-dialog.png

*Rotating the vertices by 45 degrees*

.. image:: /images/basics/rotate-result.png


Textures
--------

Sidedefs
^^^^^^^^

A Sidedef refers to the texture data for a Linedef, it can have **lower**, **middle** and **upper** textures.

The relation of the sidedefs are best illustrated with these poorly-matched textures:

.. image:: /images/basics/textures-sidedefs-3d.png

*Lower texture is COMPBLUE, middle is MIDGRATE, and upper texture is BRICK10*


**To change the sidedefs**

* Switch to 2D mode
* Enter Linedef mode (:kbd:`l`)
* Select one (or more) linedefs

.. image:: /images/basics/textures-selection.png

* Click the "Front sidedef" texture button to open the texture browser
* (optionally) Press :kbd:`tab` to switch to 3D view for a live preview
* Select a texture in the browser window

.. image:: /images/basics/textures-browser.png


Pro Tip: You can copy-paste Sidedefs quickly by hiliting the master Linedef to copy, hovering over the target Linedef and pressing the :kbd:`c` key. For this to work you must only have the one Linedef selected.


Floor / Ceiling Textures
^^^^^^^^^^^^^^^^^^^^^^^^

Enter Sector editing mode and select the sector to change:

.. image:: /images/basics/floor-ceil-texture-2d.png

Click the texture buttons to open the texture browser:

.. image:: /images/basics/floor-ceil-buttons-closeup.png

You can enter the 3D view to see a preview of the texture changes:

.. image:: /images/basics/floor-ceil-browser.png

Pro Tip: You can copy-paste ceiling and floor textures quickly by hiliting the master sector, hovering over the target sector and pressing the :kbd:`c` key.


Creating Sectors
----------------

There are two ways to create a new sector in the 2D view:

1. Enter Sector edit mode, hover the mouse cursor where the new sector is to be placed and press :kbd:`space` or :kbd:`insert`.

.. image:: /images/basics/create-sector-shortcut.png

2. Enter Vertice edit mode, use the :kbd:`RMB` to begin a line drawing operation, adding points until the new sector is closed. Enabling grid snapping will assist in placing the vertices.

.. image:: /images/basics/create-sector-vertices.png

Expanding Sectors
-----------------

Switch to Vertice edit mode and use the :kbd:`RMB` to insert a new vertice on one side of the room, add a second vertice to the Linedef on the opposite side of the room. A new Linedef is created between the two vertices.

.. image:: /images/basics/split-room.png


Floor / Ceiling Height
----------------------

Enter Sector editing mode and select the sector to change:

.. image:: /images/basics/floor-ceil-height-2d.png

Switch to 3D view and use the ceiling and floor height :kbd:`+/-` buttons:

.. image:: /images/basics/floor-ceil-buttons-closeup.png

.. image:: /images/basics/floor-ceiling-heights.png

These shortcuts can be used:

* :kbd:`,.` adjust floor height (hold shift for small increments)
* :kbd:`[]` adjust ceiling height (hold shift for small increments)

Joining Sectors
---------------

Enter Vertice edit mode and use the :kbd:`RMB` to insert vertices that bridge the sectors.

.. image:: /images/basics/join-sectors-via-vertices.png
