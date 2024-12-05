# Just Another Halo Repair Script - JAHRS
This is a Pixinsight script for repairing medium sized halos around stars.
The script will display any available image window in its image window frame.
The user can select an ellipse to place a ring around the offending halo (shift button down, and left mouse button down and drag).
The user may also use a single click and mouse button
release and the radius in the slider on the interface will be used. Also, once the user has initially selected the ellipse with the shift-left click
and the action is executed, the halo size should update on the slider.

If the selection is imperfect, either Ctrl+left mouse button will modify the selection, or start over by shift+left mouse button as above.

Once the selection is made, the execute button will modify the image window open in Pixinsight as well as that image displayed in the image preview
in the script. The Undo button undoes the changes in both the preview window and the image window open in the main Pixinsight window.

This script works on both RGB and mono images.

The Residual star slider is the size of the star that remains after the halo has been repaired. If it is set to 0, no residual star is created.

## Images

This is a sample pair of images.

<img src="./figs/Repaired flat.png" text='Repaired flat' align=left />

## Script

This is the script interface.

<img src="./figs/DonutRepairScript.png" text='Dust donut repair script' align=left />

## Manage repository location

In order to automatically refresh the script in Pixinsight, add this following to Resources > Updates > Manage repositories

https://raw.githubusercontent.com/chickadeebird/Star-Halo-Pixinsight-updates/main/

After this has been added to the repositories, Check for updates should place the new JAHRsHaloRepair script in Scripts > ChickadeeScripts
