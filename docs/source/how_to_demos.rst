.. _how_to_demos:

"How to" demos
==============

.. note:: This section is under construction. Some elements in the videos may slightly differ from what the user actually see in the rendering of the current software. We apologise for the inconvenience.

In this section we display example videos that should intuitively explain how to use iDaVIE.

Explore a cube
^^^^^^^^^^^^^^

Using the controls described in :ref:`how_to_interact`, the user can zoom in on the data and move the data where needed using the grip buttons. Then with the A button (if the primary hand is the right) or the X button (if the primary hand is the left) the user can select a region around a point of interest. The user can then use the voice command "Crop selection" to crop the cube to the region selected.

.. raw:: html

    <video controls loop style="width:100%;height:auto;">
      <source src="_static/Demo-selection-RGBaxis.mp4" type="video/mp4">
    </video>

The 3D cursor will provide information about the current voxel under the cursor. If a mask is loaded, then the cursor info will also provide feedback on the identified sources, for example:

.. raw:: html

    <img src="_static/Cursor-feedback.png"
         style="width:100%;height:auto;">


Take snapshots
^^^^^^^^^^^^^^
iDaVIE allows the user to take a "screenshot" of their current view in the VR environment, saved to :literal:`Outputs\Camera\Screenshot_yyyyMMdd_Hmmss.png`, where :literal:`yyyyMMdd_Hmmss` is the current timestamp. To do so, the user can do any of the following:

#. Invoke the quick menu and laser on the camera icon and press the trigger (of the primary hand) while looking in the direction of the area of interest (i.e., if the user looks at the menu when pressing the trigger, then the picture will contain only the menu).

#. While looking at the area of interest, the user can say "take picture". If the image was taken sucessfully, the user will receive haptic feedback (vibration) on the primary hand controller.

Create/modify/save a mask
^^^^^^^^^^^^^^^^^^^^^^^^^
iDaVIE allows the user to create a mask or to modify an existing mask in VR. Both can be done using the "Paint menu" action that can be invoked from the "Quick menu" by lasering the brush icon. Using the functionality available in the "Paint menu", the user can add or delete mask voxels using the controllers. Once done, the user can save the created/updated mask by either overwriting an existing mask or creating a new one. As also explained in :ref:`inputs_outputs`:

* if a mask is loaded and modified in VR, then it can be saved by either overwriting the original mask **or**  as a copy. In the former case, the mask will be saved with the same name of the original mask and in the same directory, while in the latter case, the suffix :literal:`-copy.fits` will be added to the original mask name and the edited mask will be saved in the same directory as the original mask (i.e., the edited mask file name will then be :literal:`originalmaskname-copy.fits`).
* if no mask is provided in input, but one is created in iDaVIE, then the created mask is saved in the same directory of the data cube and a suffix :literal:`-mask.fits` will be added to the cube name to indicate the mask file (e.g. the created mask file name will then be :literal:`originalcubename-mask.fits`).

**Demo TBD**

Interact with catalogs in VR
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
iDaVIE allows the user to load catalogs from the Desktop GUI and overplot them on the visualised data cube.

.. raw:: html

    <video controls loop style="width:100%;height:auto;">
      <source src="_static/Demo-catalogue-allthree.mp4" type="video/mp4">
    </video>

Create statistics and save moment maps
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
iDaVIE allows the user to investigate the basic statistics of the cube and to create both moment 0 and moment 1 maps of a data cube. The user can create the moment maps for the entire cube or for a single selected region. In case a mask is available, the moment maps thresholds are set by the mask, but they can be changed manually. If no mask is available, then the thresholds should be set manually using the options available in the moment map windows. The moment maps can then be saved as png.

.. raw:: html

    <video controls loop style="width:100%;height:auto;">
      <source src="_static/Demo-mmaps-Threshold.mp4" type="video/mp4">
    </video>


.. raw:: html

    <img src="_static/MMap-slide.png"
         style="width:100%;height:auto;">


Create a movie (using external tools)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
TBD
