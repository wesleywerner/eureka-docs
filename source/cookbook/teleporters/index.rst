Teleporters
===========

.. image:: teleport-01.png

A teleport is triggered by walking over a linedef with the teleport special. The tag of the linedef points to the sector where the teleport lands.

Teleport Platform
-----------------

* Create a 64x64 sector for the teleport platform
* Set the floor texture as `GATE1`, the ceiling as `TLITE6_5`
.. image:: teleport-02.png
* Enter linedef edit mode (:kbd:`l`)
* Press :kbd:`;` then :kbd:`f` to apply a fresh tag to all four linedefs. This will point to the teleport landing sector.
.. image:: teleport-03.png
* Choose the linedef **Type** as `97 WR Teleport`

.. note::

    A teleport is only triggered when walking from the **Front** to the **Back** of a linedef. This is intentional as it allows the player to walk off the landing platform without triggering another unintended teleport.

Landing Site
------------

* Tag the landing sector the same as the teleporter linedefs. Press :kbd:`;` then :kbd:`l` to apply the last used tag to the landing sector.
* Enter Thing edit mode (:kbd:`t`), position the mouse cursor inside the landing sector and press :kbd:`ins`. Choose the **Type** as `14 Teleport Exit` (labelled as TFOG in the thing browser)
.. image:: teleport-04.png
* Click the directional arrows to set the angle of the `TFOG` thing. This is the angle faced after teleporting.

Downloads
---------

:download:`teleporters.wad`
