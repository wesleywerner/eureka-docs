Project Management
==================

Your WAD can contain multiple maps, and their numbering is determined by the source IWAD you choose to use.

For Doom1, or Freedoom1, you get 4 episodes of 9 maps each: E1M1-9, E2M1-9, E3M1-9 and E4M1-9.

For Doom2, or Freedoom2, you get 32 maps: MAP01 - MAP32.

This manual will focus on the Freedoom1 IWAD.

Create a new WAD
----------------

Use the **File -> New Project** menu to create a new WAD, choose the location and file name, click OK.

Next select the settings for you new project:

* IWAD: pick freedoom1 from the list, use the **Find** button if you need to browse for it
* Source Port: pick boom (or your nearest source port) from the list, use the **Setup** button to browse for the executable
* If you are a GNU / Linux user, you can find the location of the executable with the bash command ``which prboom``.

Click **OK** when done.

.. image:: new-project-dialog.png

Open a map
----------

Use the :kbd:`File -> Open Map` menu or press :kbd:`control-o`. Make sure you pick **Find map in the PWAD above**, otherwise you will be modifying the maps from the freedoom1 IWAD.

.. image:: open-map.png


Add a new map
-------------

Use the :kbd:`File -> Fresh Map` menu, you are prompted to pick the slot where the new map will be placed, green slots are empty and red slots already contain maps.

.. image:: fresh-map-dialog.png

Rename a map
------------

Use the :kbd:`File -> Rename Map` menu to change the play order of a map, a dialog prompts you to pick the new slot for the map.

Slots with existing maps cannot be selected.

.. image:: rename-map-dialog.png

Copy a map
----------

Use the :kbd:`File -> Copy Map` menu to copy the current map to another slot.

Delete a map
------------

Use the :kbd:`File -> Delete Map` menu to remove the current map from the WAD. You will be prompted to confirm the delete.

Export a map
------------

Use the :kbd:`File -> Export Map` menu to export the current map to:

* a new WAD
* an existing WAD

.. image:: export-map-file-chooser.png

*Pick the file to export to*

.. image:: export-map-level-chooser.png

*Select the level of the exported map*

