User Interface
==============

Eureka features a 2D orthogonal view and a 3D view. Switch between the two views with the :kbd:`tab` key.

.. image:: 2d-view.png

*The 2D view is used to construct walls and place things on the map*

.. image:: 3d-view.png

*The 3D view is used to preview textures and make ceiling, floor and light adjustments*

Panning and Zooming
-------------------

To move around the 2D view:

* Roll the mouse wheel to zoom
* Click and drag with the middle mouse button (mouse wheel) to pan
* Press :kbd:`home` to zoom the whole map into view

The Camera
----------

This arrow in 2D view indicates the current position of the 3D camera.

* Press :kbd:`'` (single quote) in the 2D view to position the 3D camera at the location of the mouse cursor.
* Press :kbd:`end` in 2D view to center the map on the camera position.

.. image:: camera.png

When in the 3D view you can control camera movement with the following controls:

* Roll the mouse wheel to move forward/backward
* Click and drag left/right with the middle mouse button to rotate the view
* Click and drag up/down with the middle mouse button to raise/lower the view

The Grid
--------

Toggle the grid in 2D view with the **Grid** dropdown box (located on the bottom status bar), or by pressing :kbd:`g`. You can quickly change the grid size with the :kbd:`0-9` keys.

Toggle free mode / grid snapping with the :kbd:`f` key.

.. image:: 2d-grid.png

.. note::

    If you encounter lag while panning a large zoomed-out map, disable grid rendering with :kbd:`g` while panning.

Rendering Mode
--------------

The 2D View can render sectors to display their floor or ceiling flats, light levels or sound propagation. You can change the sector rending mode by using the `Rend` dropdown on the status bar, or by pressing the :kbd:`F8` key to bring up the rendering popup.

The status bar dropdown:

.. image:: sector-rendering-dropdown.png

The :kbd:`F8` popup menu:

.. image:: sector-rendering-statusbar.png

Floor sector rendering
^^^^^^^^^^^^^^^^^^^^^^

This mode draws the floor textures of sectors.

.. image:: sector-rendering-floors.png

Ceiling sector rendering
^^^^^^^^^^^^^^^^^^^^^^^^

This mode draws the ceiling textures of sectors.

.. image:: sector-rendering-ceilings.png

Lighting sector rendering
^^^^^^^^^^^^^^^^^^^^^^^^^

The light render mode draws shades of sector light levels.

.. image:: sector-rendering-lighting.png

Sound sector rendering
^^^^^^^^^^^^^^^^^^^^^^

The sound render mode highlights sectors based on how sound travels. You have to be in sector edit mode for this mode to work (press :kbd:`s`), hover your mouse cursor over a sector to see how sound will propagate.

* Orange sectors indicate where sound will reach at volume 2, the initial and loudest volume.
* Red sectors indicate where sound will reach at volume 1.
* Blue sectors indicate sectors where sound does not reach.

When sound travels across a Linedef that has the `sound block` flag set, the volume is reduced by 1. Thus sound travelling across two or more blocking Linedefs will not be heard by monsters.
By setting the `sound block` flag on Linedefs, you can lower the volume of traveling sounds. Sounds do not travel across two sound-blocking lines.

.. image:: sector-rendering-sound.png

The sound block flag on a Linedef:

.. image:: sector-rendering-sound-flag.png


Find and Replace
----------------

Open the find panel with the `View / Find` menu or press :kbd:`control-f`.

You can search for Things, line textures, sector flats, lines by type (specials) or sectors by type.

.. image:: find-panel.png

Alternative key bindings
------------------------

This section lists some alternative key bindings you may find useful, while demonstrating how key bindings can be changed or added.

**mouselook in 3D view**

This setting will enable horizontal left/right camera rotation (mouselook) while holding the right mouse button, and vertical up/down motion while holding the right mouse button.

* Open Preference, Keys tab, click the Add button
* Click the Rebind button followed by the right mouse button (MOUSE3)
* Choose the Function as `2D View/NAV_MouseScroll`
* Choose the Mode as 3D View
* Enter Params as `1`
* Click OK

**Adjust light levels with the mouse scroll wheel**

This setting allows you to adjust the light level of the selected Sector by holding shift and scrolling the mouse wheel.

* Open Preference, Keys tab, click the Add button
* Click the Rebind button, hold shift and scroll the mouse wheel Up
* Choose the Function as `Sector/SEC_Light`
* Enter Params as `8`
* Click OK and click Add again
* Click the Rebind button, hold shift and scroll the mouse wheel Down
* Choose the Function as `Sector/SEC_Light`
* Enter Params as `-8`
* Click OK

**Enhance 2D grid display**

This setting increases the grid visibility and make it easier to distinguish the grid scale in 2D view.

* Open Preference, Grid tab
* Change the Grid style to Dotty
* Hover over the Dotty grid colors to locate the "dot color"
* Change the color to a high visibility hue (cyan for example, is hue 3)
