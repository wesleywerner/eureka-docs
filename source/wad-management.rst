WAD Management
==============

You need an IWAD file to play any stock Doom engine, this file contains the default game levels, textures, sounds and other auxiliary data.

A PWAD (Patch WAD) provides additional levels and other resources that replace those in the IWAD. When making levels in Eureka we will be working with PWADs, any mention of WAD implies the PWAD unless otherwise mentioned.

Create a new WAD
----------------

Use the **File -> New Project** menu to create a new WAD, choose the location and file name, click OK.

Next select the settings for you new project:

* IWAD: pick freedoom1 from the list, use the **Find** button if you need to browse for it
* Source Port: pick boom from the list, use the **Setup** button to browse for the executable
* If you are a GNU / Linux user, you can find the location of the executable with the bash command ``which prboom``.

Click **OK** when done.

.. image:: /images/wad-management/new-project-dialog.png

Open a map
----------

Use the :kbd:`File -> Open Map` menu or press :kbd:`Control-o`. Make sure you pick **Find map in the PWAD above**, otherwise you will be modifying the maps from the freedoom1 IWAD.

.. image:: /images/wad-management/open-map.png


Add a new map
-------------

Use the :kbd:`File -> Fresh Map` menu, you are prompted to pick the slot where the new map will be placed, green slots are empty and red slots already contain maps.

.. image:: /images/wad-management/fresh-map-dialog.png

Change the play order
---------------------

Use the :kbd:`File -> Rename Map` menu to change the play order of a map, a dialog prompts you to pick the new slot for the map.

Slots with existing maps cannot be selected.

.. image:: /images/wad-management/rename-map-dialog.png

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

.. image:: /images/wad-management/export-map-file-chooser.png

*Pick the file to export to*

.. image:: /images/wad-management/export-map-level-chooser.png

*Select the level of the exported map*

