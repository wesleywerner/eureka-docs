Building Basics
===============

.. note::

    LMB: left mouse button click, RMB: right mouse button click

To follow these building basics, create a new project in Eureka.

Adding a room
-------------

To help with drawing, press :kbd:`f` to toggle grid snapping, press :kbd:`g` to enable grid display, and press :kbd:`5` to set the grid size to 32 units.

* Press :kbd:`tab` to switch to the 2D view
* Press :kbd:`v` to enter vertices edit mode
* Use the :kbd:`RMB` to draw a new sector. Make sure to keep adding vertices with the right mouse button, and to close the sector.

.. image:: adding-01.png

**Texturing the new walls**

Press :kbd:`l` to enter linedef edit mode. The new linedefs should be selected, if not click with the LMB and drag a box around them to select.

.. image:: adding-02.png

* Position the mouse cursor inside your new sector and press :kbd:`'` to place the camera inside the room.
* Press :kbd:`tab` to enter 3D view
* Click the front sidedef texture button and pick the SLADWALL texture.

.. image:: adding-04.png
.. image:: adding-03.png

**Texturing the new floor and ceiling**

* Press :kbd:`tab` to return to 2D view
* Press :kbd:`s` to enter sector edit mode. The new sector should remain selected, if not click the LMB to select it.
* Press :kbd:`tab` to return to the 3D view
* Click on both the **Floor** and **Ceiling** texture buttons, and select the FLOOR5_1 texture.

.. image:: adding-05.png
.. image:: adding-06.png

Joining rooms
-------------

* Press :kbd:`tab` to enter 2D view
* Press :kbd:`v` for vertices edit mode
* Click with the :kbd:`RMB` to insert vertices that bridge the neighbouring sectors
* Make the line of the doorway 128 units in length, this is the size of the wide door texture
* When the join is complete, the rooms are connected

.. image:: joining-01.png
.. image:: joining-02.png

Adjusting ceiling height
------------------------

* Press :kbd:`tab` to enter 2D view
* Press :kbd:`s` for sector edit mode
* Select the sector you want to adjust

.. image:: joining-03.png

* Press :kbd:`tab` to return to 3D view
* Click the ceiling `+-` buttons to adjust the ceiling height

.. image:: joining-04.png

* Alternatively press :kbd:`[]` to adjust ceiling height via keyboard shortcuts

.. image:: joining-05.png

Texture alignment
-----------------

* Press :kbd:`tab` to enter 3D view
* Click with the :kbd:`LMB` to select walls with misaligned textures

.. image:: alignment-01.png

* Press these keyboard shortcuts to align:
    * :kbd:`x`: align X offset with wall to the left
    * :kbd:`y`: align Y offset with wall to the left
    * :kbd:`z`: align both X and Y offsets with wall to the left
    * :kbd:`shift-x`: align X offset with wall to the right
    * :kbd:`shift-y`: align Y offset with wall to the right
    * :kbd:`shift-z`: align both X and Y offsets with wall to the right

* Alternatively press :kbd:`F1` to open the operations menu and select one of the align options.

.. image:: alignment-02.png

Auto alignment
--------------

If you need to align multiple surfaces, you can use the auto-align feature:

* In the 2D view, enter linedef edit mode :kbd:`l`
* Highlight all lines to align
* Press :kbd:`shift-A` to auto-align offsets on all selected linedefs
* This shortcut works in both 2D and 3D views
