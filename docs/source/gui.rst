.. _gui:

Graphical User Interface
========================
.. note:: This section is under construction. We apologies for the inconvenience. 

iDaVIE-v presents two sets of GUIs: the :literal:`Desktop GUI` which is the one the user will interact with while at the computer/desktop using the keybord and the :literal:`VR GUI` which is the one the user will interact with in the VR environment using the VR controllers. 

Desktop GUI
-----------
This is the GUI that the user use to start the VR session. It is the first thing that appear to the user on the computer screen when iDaVIE-v.exe is executed. 

.. raw:: html

    <img src="_static/Desk_GUI1.png"
         style="width:100%;height:auto;">

Using this GUI the user can load the “data cube” of its choice pressing the “Browse” button on the “Image File” line.

**NOTE:** Users can also loads cube that have 4 dimensions. If a cube with four dimensions is loaded the system will give the opportunity to choose which axis (3 or 4) to use based on the header of the cube. To choose the Z axis a drop down menu will appear for the z axis selection.

.. raw:: html

    <img src="_static/Desk_GUI2.png"
         style="width:100%;height:auto;">

Once the cube is loaded the user can do one or more of the following actions:

#. Check the header of the cube reported in the grey rectangule (in order to check whether the software has interpreted it correctly).

#. Tune the rendering of the cube using the options in the RENDERING tab or check some basics stats of the cube (this can also be done using the Main Menu options in the VR GUI)

#. Load a mask file (if any) by pressing the “Browse” button on the “Mask File” line. NOTE: the mask must have the same dimensions of the cube loaded. See below, both the FITS cube and the mask have been selected. Now you are ready to Load and render.

   .. raw:: html

       <img src="_static/Desk_GUI3.png"
            style="width:100%;height:auto;">

#. Load a catalog of sources (if any) using the "SOURCES" tab. In this case the user will need to indicate which columns needs to be imported and which columns are ID, Right ascension, Declination and redshifts. These latter are essential columns to proceed with the 3D rendering of the catalog.

   .. raw:: html

       <img src="_static/Desk_GUI4.png"
            style="width:100%;height:auto;">

#. Skip all the previous step and just press "Load". Once this is done the user can wear the headset and start exploring the cube. The first look the user will see is something like this:

   .. raw:: html

       <img src="_static/VR-first-view.png"
            style="width:100%;height:auto;">

   Axes are RGB color coded as:
   
   Red, Green = X, Y (e.g. RA, DEC respectively)
   
   Blue = Z (e.g velocity, redshift)
    

VR GUI
------
TBD

Main menu
^^^^^^^^^
TBD

Quick menu
^^^^^^^^^^
TBD

Mask painting menu
^^^^^^^^^^^^^^^^^^
TBD

Saving menu
^^^^^^^^^^^
TBD

Stats & Moment maps menu
^^^^^^^^^^^^^^^^^^^^^^^^
TBD