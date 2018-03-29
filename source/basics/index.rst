Building Basics
===============

Creating Sectors
----------------

There are two ways to create a new sector in the 2D view:

1. Enter Sector edit mode, hover the mouse cursor where the new sector is to be placed and press :kbd:`space` or :kbd:`insert`.

.. image:: create-sector-shortcut.png

2. Enter vertex edit mode, use the :kbd:`RMB` to begin a line drawing operation, adding points until the new sector is closed. Enabling grid snapping will assist in placing the vertices.

.. image:: create-sector-vertices.png

Expanding Sectors
-----------------

Switch to vertex edit mode and use the :kbd:`RMB` to insert a new vertex on one side of the room, add a second vertex to the Linedef on the opposite side of the room. A new Linedef is created between the two vertices.

.. image:: split-room.png


Floor / Ceiling Height
----------------------

Enter Sector editing mode and select the sector to change:

.. image:: floor-ceil-height-2d.png

Switch to 3D view and use the ceiling and floor height :kbd:`+/-` buttons:

.. image:: floor-ceil-buttons-closeup.png

.. image:: floor-ceiling-heights.png

These keys can be used:

* :kbd:`,.` adjust floor height (hold shift for small increments)
* :kbd:`[]` adjust ceiling height (hold shift for small increments)

Joining Sectors
---------------

Enter vertex edit mode and use the :kbd:`RMB` to insert vertices that bridge the sectors.

.. image:: join-sectors-via-vertices.png
