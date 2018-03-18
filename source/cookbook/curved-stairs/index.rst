Curved Stairs
=============

.. image:: capture_001.jpg

Layout
------

.. image:: capture_002.png


Method
------

Draw the outline of the stairs in vertex edit mode:

.. image:: capture_003.png

Use the :kbd:`LMB` to insert vertices along the edges, to define where the steps will be:

.. image:: capture_004.png

Press :kbd:`f` to toggle free mode (no grid snapping) and drag the step vertices *roughly* into the arc shape.

.. image:: capture_005.png

Deselect all vertices (:kbd:`\``) and only select those on one side of the stairs:

.. image:: capture_006.png

Press :kbd:`shift-c` (shape arc to 120 degrees):

.. image:: capture_007.png

Now deselect all vertices, select only the other side and apply the shape arc operation again. Next use the :kbd:`RMB` to join the step vertices:

.. image:: capture_009.png

Switch to sector edit mode, hold :kbd:`shift` and drag-select the stair sectors:

.. image:: capture_010.png

Press the raise floor shortcut (:kbd:`.`) twice. Using the :kbd:`LMB`, deselect the left-most step, and deselect the right-most step:

.. image:: capture_011.png

* Repeat raising the floor and deselecting a step from either side, until you reach the center step. Your stairs are now done:

.. image:: capture_012.png


Notes
-----

The shape arc operation is also available by pressing :kbd:`f1` to bring up the operations menu. However this menu does not have the 120 degree arc, so we used the :kbd:`shift-c` keyboard shortcut.

.. image:: capture_008.png


Downloads
---------

:download:`curved-stairs.wad`
