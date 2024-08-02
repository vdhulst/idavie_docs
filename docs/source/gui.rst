.. _gui:

Graphical User Interface
========================
.. note:: This section is under construction. We apologies for the inconvenience. 

iDaVIE presents two types of GUI: the :literal:`Desktop GUI`, which is the one the user will interact with while at the computer/desktop using the keyboard, and the :literal:`VR GUI`, which is the one the user will interact with in the VR environment using the VR controllers.

Desktop GUI
-----------
This is the GUI that the user uses to start the VR session. It is the first thing that appears to the user on the computer screen when iDaVIE.exe is executed. 

.. raw:: html

    <img src="_static/Desk_GUI1.png"
         style="width:100%;height:auto;">

Using this GUI the user can load the “data cube” of their choice by pressing the “Browse” button on the “Image File” line.

**NOTE:** Users can also load cube that have 4 dimensions. If a cube with four dimensions is loaded, the system will give the opportunity to choose which axis (3 or 4) to use based on the header of the cube. To select the Z axis, a drop down menu will appear listing the axes.

.. raw:: html

    <img src="_static/Desk_GUI2.png"
         style="width:100%;height:auto;">

Once the cube is loaded, the user can do one or more of the following actions:

#. Check the header of the cube reported in the grey rectangle (in order to check if the software has interpreted the header correctly).

#. Tune the rendering of the cube using the options in the RENDERING tab or check some basics stats of the cube (these can also be done through the Main Menu options in the VR GUI)

   .. raw:: html

        <img src="_static/GUI_thresholds.png"
             style="width:100%;height:auto;">

   .. raw:: html

        <img src="_static/GUI-stats-histogram.png"
             style="width:100%;height:auto;">
     

#. Load a mask file (if any) by pressing the “Browse” button on the “Mask File” line. NOTE: the mask must have the same dimensions of the cube loaded. See below, both the FITS cube and the mask have been selected. Press the :literal:`Load` button to start the render process.

   .. raw:: html

       <img src="_static/Desk_GUI3.png"
            style="width:100%;height:auto;">

#. Load a catalog of sources (if any) using the "SOURCES" tab. In this case, the user will need to indicate which columns (of the catalog) need to be imported, and must indicate which columns correspond to the :literal:`ID`, :literal:`Right ascension`, :literal:`Declination`, and :literal:`redshift`. These are mandatory columns to proceed with the 3D rendering of the catalog.

   .. raw:: html

       <img src="_static/Desk_GUI4.png"
            style="width:100%;height:auto;">

#. Skip all the previous steps and just press "Load". Once this is done the user can wear the headset and start exploring the cube. The first image the user will see is something like this:

   .. raw:: html

       <img src="_static/VR-first-view.png"
            style="width:100%;height:auto;">

   The axes are RGB color coded as:
   
   Red, Green = X, Y (e.g., RA, DEC respectively)
   
   Blue = Z (e.g., velocity or redshift)
    

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