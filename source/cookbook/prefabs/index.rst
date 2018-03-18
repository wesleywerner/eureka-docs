Prefabs
=======

Prefabs are useful to quickly throw maps together by copy-pasting predesigned structures.

.. image:: capture_001.png

Things to keep in mind when using prefabs:

1. You can only copy-paste in the same Eureka instance.
2. You have to merge common vertices and sectors after pasting.

Exporting your prefab map to an unused slot in your game wad allows quicker switching.

Downloads
---------

Use :download:`prefabs.wad` as a base for adding your own designs.

.. image:: capture_002.png

Merging Vertices
----------------

Copying a prefab into void space, like a door prefab, needs vertice merging.

Select the door prefab in sector mode, press :kbd:`control-c`:

.. image:: capture_003.png

Open the target map, position the mouse cursor where you want the prefab and paste with :kbd:`control-v`:

.. image:: capture_004.png

Enter vertice edit mode, use the :kbd:`RMB` to link the room with the door vertices:

.. image:: capture_005.png

If you optionally want to get rid of the extra sector in between, select the one room vertice, then the matching door vertice (this order matters) and merge them:

.. image:: capture_006.png

Do the same for the other vertices (selecting the room vertice first):

.. image:: capture_007.png

This completes your door:

.. image:: capture_008.png

Merging Sectors
---------------

The process of pasting sectors into sectors requires another kind of merging. The stairs prefab is one such example.

Select the prefab sectors. You might need to use :kbd:`shift LMB` to avoid dragging sectors during selection:

.. image:: capture_009.png

Copy, open your map, and paste. Ensure your mouse cursor is positioned where you want the prefab pasted:

.. image:: capture_010.png

Switching to 3D view shows us artifacts, the prefab needs merging first:

.. image:: capture_011.png

To merge, unselect everything (:kbd:`\``), hover to hilight the room sector and press :kbd:`space`:

.. image:: capture_012.png

The stairs prefab is now merged with your room sector:

.. image:: capture_013.png
