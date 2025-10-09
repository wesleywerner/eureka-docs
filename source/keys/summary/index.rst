Keyboard and Mouse Summary
==========================

Note: on macOS, the **CTRL** key gets replaced by the Command key, and **META** by the Control key.

All Modes
---------

Cursor keys : scroll the map

**MOUSE1** (LMB)

- select an object, drag to move the object(s)
- click in an empty area to clear the selection
- click + drag in empty area to select a group of objects

**MOUSE2** (MMB)

- scroll the map around (by dragging)

**MOUSE3** (RMB)

- begin/continue line drawing (in vertex mode)
- merge sectors (in sectors mode)
- with CTRL pressed: bring up operation menu

**WHEEL** : zoom in or out

**MENU** : operation menu

**TAB** : toggle the 3D view on or off

**t** : enter Thing mode

**l** : enter Linedef mode

**s** : enter Sector mode

**v** : enter Vertex mode

**b** : toggle the Browser on or off

**1** .. **9** : select the grid size (smallest to largest)

**CTRL**-**z** : undo (can be used multiple times)

**CTRL**-**y** : redo (i.e. undo the previous undo)

**CTRL**-**a** : select all

**CTRL**-**i** : invert the selection

**CTRL**-**u** : clear the selection

**`** (backquote) : clear the selection

**HOME** : move/zoom 2D viewport to show the whole map

**END** :  move 2D viewport to camera location

**'** (quote) : move 3D camera to position of mouse pointer

**f** : toggle free mode vs grid snapping

**g** : toggle grid on / off

**N** : open next map in the current wad

**P** : open previous map in the current wad

**j** : jump to object (by its numeric id)

**J** : toggle object number display

**o** : copy and paste the selected objects

**c** : copy properties from selected --> highlighted object

**C** : copy properties from highlighted --> selected objects

**H** : mirror objects horizontally

**V** : mirror objects vertically

**a** : scroll map with the mouse

**r** : scale selected objects with the mouse

**R** : scale selected objects, allow stretching

**CTRL**-**r** : rotate the selected objects (with the mouse)

**K** : skew (shear) the selected objects

**\\** : toggle the RECENT category in the Browser

**;** : make the next key pressed META

**META**-**n** : load next file in given list

**META**-**p** : load previous file in given list

**META**-**f** : apply a fresh tag to the current objects

**META**-**l** : apply the last (highest) tag to the current objects

Things Mode
-----------

**SPACE** : add a new thing

**w** : rotate things 45 degrees anti-clockwise

**x** : rotate things 45 degrees clockwise

**d** : disconnect things at the same location

**m** : move selected things to occupy the same location

Vertex Mode
-----------

**SPACE**

- begin/continue line drawing
- with **SHIFT** pressed: continue in drawing mode
- with **CTRL** pressed: inhibit creation of sectors

**d** : disconnect all linedefs at the selected vertices

**m** : merge selected vertices into a single one

**I** : reshape selected vertices into a line

**O** : reshape selected vertices into a circle

**D** : reshape selected vertices into a half-circle

**C** : reshape selected vertices into a 120-degree arc

**Q** : reshape selected vertices into a 240-degree arc

Linedef Mode
------------

**e** : select a chain of linedefs

**E** : select a chain of linedefs with same textures

**w** : flip linedefs

**k** : split linedefs in two

**A** : auto-align offsets on all selected linedefs

**d** : disconnect selected linedefs from the rest

**m** : merge two one-sided linedefs into a two-sided linedef

Sector Mode
-----------

**SPACE**

- add a new sector to area around the mouse pointer
- if a sector is selected, copy that sector instead of using defaults

**d** : disconnect sector(s) from their neighbors

**m** : merge all selected sectors into a single one

**e** : select sectors with same floor height

**E** : select sectors with same floor texture

**D** : select sectors with same ceiling texture

**w** : swap floor and ceiling textures

**,** and **<** : lower floor heights

**.** and **>** : raise floor heights

**[** and **{** : lower ceiling heights

**]** and **}** : raise ceiling heights

3D Preview
----------

Cursor keys : move forward and back, turn left and right
(the WASD keys can also be used for moving around the map)

**MOUSE1** (LMB) : select walls, floors or ceilings

**MOUSE2** (MMB) : turn or move the camera (by dragging the mouse)

**WHEEL** : move camera forwards or backwards

**PGUP** and **PGDN** : move camera up and down

**g** : toggle gravity (i.e. as if the player was walking on the ground)

**v** : drop to the ground

**r** : adjust offsets on highlighted wall (by dragging the mouse)

**c** : clear offsets on highlighted sidedef

**x** : align X offset with wall to the left

**y** : align Y offset with wall to the left

**z** : align both X and Y offsets

**X** : align X offset with wall to the right

**Y** : align Y offset with wall to the right

**Z** : align both X and Y offsets

**F11** : increase brightness (gamma)

**l**  : toggle lighting on or off

**t**  : toggle texturing on or off

**o**  : toggle objects on or off
