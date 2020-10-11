Lifts
=====

.. image:: lifts-01.png

Method
------

* Enter vertex edit mode and create the lift platform. This can be a simple split of a raised sector:

.. image:: lifts-05.png

* Ensure the Linedef on the front of the lift is facing outward. A lift is triggered from the **Front** Linedef.
* If the Linedef is facing the wrong way, you can select it and press :kbd:`F1` for the operations menu, and select `Flip`:

.. image:: lifts-06.png

* Enter Linedef edit mode, select the front of the lift

.. image:: lifts-02.png

* Choose the **Type** as `62 SR Lower Lift`
* Press :kbd:`;` then :kbd:`f` to apply a fresh tag to the Linedef

.. image:: lifts-03.png

* Enter sector edit mode (:kbd:`s`), select the lift sector
* Press :kbd:`;` then :kbd:`l` to apply the last tag to the sector

.. image:: lifts-04.png

.. note::

    The SR line special indicates Switch Repeating, so the lift can be used over and over.

Downloads
---------

:download:`lifts.wad`
