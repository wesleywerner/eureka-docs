Mapping Concepts
================

.. note::

    LMB: left mouse button click, RMB: right mouse button click

Vertices
--------

Vertices are the joins between Lines, and the corners between walls.

* Press :kbd:`v` in the 2D view to enter Vertices edit mode
* :kbd:`LMB` while hovering over a Linedef inserts a single vertex at the cursor position
* :kbd:`RMB` inserts a vertex in **line drawing** mode, keep adding vertices with :kbd:`RMB` until you close the polygon

.. image:: vertices.png

Linedefs
--------

Linedefs divide the map into sectors, and they are also used to trigger actions.

Press :kbd:`l` in the 2D view to enter Linedef edit mode.

.. image:: linedefs.png

A linedef also has a front and a back. You can tell the front of a Linedef by the direction of the protruding pin in the middle of the Linedef.

.. image:: linedef-front.png

*this linedef front is facing down*


Sectors
-------

A sector is an area defined by multiple Linedefs.

Press :kbd:`s` in the 2D view to enter Sector edit mode.

.. image:: sectors.png

Things
------

Things represent players, monsters, pick-ups, obstacles, decorations, player start positions and teleport landing sites.

Press :kbd:`t` in the 2D view to enter Things edit mode. :kbd:`space` or :kbd:`ins` inserts a new thing at the cursor position.

.. image:: things.png

Multiple Selections
-------------------

While in the 2D view, you can select Vertices, Linedefs, Sectors and Things by:

* Clicking an item to select/deselect it
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

.. image:: scale-selection.png

*Four inner most vertices are selected*

.. image:: scale-dialog.png

*Scaling the vertices by 50% on the x-axis*

.. image:: scale-result.png

Rotating
^^^^^^^^

Click on :kbd:`Edit -> Rotate Object` or press :kbd:`F4` to show the rotate dialog.

.. image:: scale-selection.png

*Four inner most vertices are selected*

.. image:: rotate-dialog.png

*Rotating the vertices by 45 degrees*

.. image:: rotate-result.png


Textures
--------

Sidedefs
^^^^^^^^

A Sidedef refers to the texture data for a Linedef, it can have **lower**, **middle** and **upper** textures.

The relation of the sidedefs are best illustrated with these poorly-matched textures:

.. image:: textures-sidedefs-3d.png

*Lower texture is COMPBLUE, middle is MIDGRATE, and upper texture is BRICK10*


**To change the sidedefs**

* Switch to 2D mode
* Enter Linedef mode (:kbd:`l`)
* Select one (or more) linedefs

.. image:: textures-selection.png

* Click the "Front sidedef" texture button to open the texture browser
* (optionally) Press :kbd:`tab` to switch to 3D view for a live preview
* Select a texture in the browser window

.. image:: textures-browser.png

Floor / Ceiling Textures
^^^^^^^^^^^^^^^^^^^^^^^^

Enter Sector editing mode and select the sector to change:

.. image:: floor-ceil-texture-2d.png

Click the texture buttons to open the texture browser:

.. image:: floor-ceil-buttons-closeup.png

You can enter the 3D view to see a preview of the texture changes:

.. image:: floor-ceil-browser.png

