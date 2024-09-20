.. _gui:

Graphical User Interface
========================
.. note:: This section is under construction. We apologies for the inconvenience. 

iDaVIE presents two types of GUI: the :literal:`Desktop GUI`, which is the one the user will interact with while at the computer/desktop using the keyboard, and the :literal:`VR GUI`, which is the one the user will interact with in the VR environment using the VR controllers.

Desktop GUI
-----------
This is the GUI that the user uses to start the VR session. It is the first thing that appears to the user on the computer screen when iDaVIE.exe is executed. 


The Desktop GUI is divided into two main sections: the left side, which includes options to 
display a view of the VR user or further information on iDaVIE, and the right side, which  functions as the
which is the main control panel. The control panel is divided into three tabs: FILE, RENDER, STATS, SOURCES and DEBUG.

Using this GUI the user can load the “data cube” of their choice by pressing the :literal:`Browse` button on the :literal:`Image File`` line.

Once the cube is loaded, the user can do one or more of the following actions:

#. Check the header of the cube reported in the grey rectangle (in order to check if the software has interpreted the header correctly).

#. Tune the rendering of the cube using the options in the RENDERING tab or check some basics stats of the cube (these can also be done through the Main Menu options in the VR GUI)

FILE tab
^^^^^^^^

The FILE tab is what the user will see when iDaVIE is opened. This tab includes the options to load a cube, load a mask, read header information of the cube, and start the VR session.

**NOTE:** Users can also load cube that have 4 dimensions. If a cube with four dimensions is loaded, the system will give the opportunity to choose which axis (3 or 4) to use based on the header of the cube. To select the Z axis, a drop down menu will appear listing the axes.

.. raw:: html

     <img src="_static/Desktop1.png"
          style="width:100%;height:auto;">

1) Button to display the desktop :literal:`VR View`. This is the view that the user will see when the VR headset is worn. VR View is activated by default upon loading the cube.
2) Button to display more iDaVIE information. This includes the version of the software, the authors, and the license.
3) Button to exit iDaVIE.
4) Click this Browse button to open the file explorer and select the cube file to load.
5) The header information for the selected data cube will be displayed here.
6) Optionally, you can click the Browse button to open the file explorer and select a mask file to load. NOTE: the mask must have the same dimensions of the cube loaded.
7) Click the Load button to start the rendering of the cube. A loading bar will appear at the bottom of the window to indicate load progress. Once this is done the user can wear the headset and start exploring the cube. 


RENDER tab
^^^^^^^^^^

The RENDER tab includes options to tune the rendering parameters of the cube.

.. raw:: html

     <img src="_static/Desktop2.png"
          style="width:100%;height:auto;">

1) Dropdown menu to set a precalculated size for the cube side lengths. The default is :literal:`X=Y=Z`, setting the cube to 1x1x1 size. The other option of :literal:`X:Y:Z`` sets the side lengths of the cube to have the same ratio as the data dimensions.
2) Dropdown menu to set the applied color map for the cube. The default is the Inferno color map.
3) Slider to adjust the minimum threshold of the cube. This sets what data value will be both the lowest end of the color map as well as an alpha value of 0.
4) Slider to adjust the maximum threshold of the cube. This sets what data value will be both the highest end of the color map as well as an alpha value of 1.
5) This button resets the thresholds to the default values.
6) Dropdown menu to set the rest frequency of the cube. This is used to convert between frequency/wavelength and velocity units for spectral cubes. In addition to the dropdown options that are defined in the config file, the :literal:`Default` option uses the rest frequency defined in the cube header (if present) while the :literal:`Custom`` option allows the user to input a custom rest frequency.
7) Input field to set the custom rest frequency. This is only available when the :literal:`Custom`` option is selected in the dropdown menu.
8) Active VR View

STATS tab
^^^^^^^^^^
The STATS tab includes options to check and interact with some basic data statistics of the cube

.. raw:: html

     <img src="_static/Desktop3.png"
          style="width:100%;height:auto;">


1) Calculated histogram of the cube data. The histogram is calculated using the minimum and maximum scales below.
2) Common percentiles to set the minimum and maximum scales of the histogram. The default is 100% (which sets 0% for the minimum).
3) Input field to set the minimum percentile of the histogram. The default is the minimum value of the cube. Press enter to update the histogram.
4) Input field to set the maximum percentile of the histogram. The default is the maximum value of the cube. Press enter to update the histogram.
5) Dropdown to mark the different sigma levels in the histogram. The default displays 1 sigma.
6) Button to set above options to the default values.


SOURCES tab
^^^^^^^^^^^

The SOURCES tab includes options to load a catalog of sources. The catalog can be in a VOTable :literal:`.xml`` format or a :literal:`.fits`` table. 

.. raw:: html

     <img src="_static/Desktop4.png"
          style="width:100%;height:auto;">

1) Click this Browse button to open the file explorer and select the catalog file to load.
2) Optionally, click this browse button to select and apply a mapping :literal:`.json` file that was saved from a previous session.
3) These are the names of the columns in the source file.
4) Dropdown menu to select where to map the indicated column. This includes position (x,y,z image coordinates or wcs astronomy coordinates) for point sources, but box corners can also be mapped (currently only for x,y,z image coordinates). A name column can also be indicated.
5) Tick this box to import the indicated column for display in the VR source info box when the source is selected in the scene.
6) Click this button to save the chosen mappings and import ticks as a :literal:`.json` file for later use.
7) Click this Load button to load the source file with the chosen mapping. This will be greyed out if sufficient mappings are not selected for position coordinates.
8) Tick this box to exlcude sources that are not within the cube bounds. This is useful for large catalogs that may extend far outside the cube.
9) Message indicating if the source file was successfully loaded.


DEBUG tab
^^^^^^^^^

The DEBUG tab includes a readout of the debug log for the current session. This is useful for troubleshooting issues with the software.


.. raw:: html
     
          <img src="_static/Desktop5.png"
               style="width:100%;height:auto;">


1) Readout of the debug log
2) Button to save the log to the Outputs directory

    

VR GUI
------
After loading a file in the FILE tab, the user can put on the headset. The first image the user sees will be something like this:

   .. raw:: html

       <img src="_static/VR-first-view.png"
            style="width:100%;height:auto;">

   The axes are RGB color coded as (for example):
   
   Red, Green = X, Y (e.g., RA, DEC respectively)
   
   Blue = Z (e.g., velocity or redshift)

Main menu
^^^^^^^^^


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

VR Controller
-------------

