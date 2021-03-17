.. _how_to_demos:

"How to" demos
==============

.. note:: This section is under construction. Some elements in the videos may slightly differ from what the user actually see in the rendering of the current software. We apologies for the inconvenience.

In this section we store example videos that should intuitively explain how to use iDaVIE-v.

Explore a cube
^^^^^^^^^^^^^^

Exploiting the controllers described in :ref:`how_to_interact` the user can zoom in on the data and move the data where needed using the grip buttons. Then with the A button (if the primary hand is the right) or the X button (if the primary hand is the left) the user can select a region around a point of interest. The user can then use the voice command "Crop selection" to crop the cube to the region selected.

.. raw:: html

    <video controls loop style="width:100%;height:auto;">
      <source src="_static/Demo-selection-RGBaxis.mp4" type="video/mp4">
    </video>

The 3D cursor will provide infos on the voxel where is located, if a mask is loaded then the cursor info will also provides feedbacks on the identified sources like in this case:

.. raw:: html

    <img src="_static/Cursor-feedback.png"
         style="width:100%;height:auto;">


Take snapshots
^^^^^^^^^^^^^^
iDaVIE-v allows to take a "screenshot" of what is in front of the user in a particular moment. To do so the user can do any of the followings:

#. invoke the quick menu and laser on the camera icon and press the trigger (of the primary hand) while paying attention to look in the direction of what is meant to be capturd in the picture (e.g. if the user looks to the menu when pressing the trigger than the picture will contain only the menu)

#. while looking to what needs to be captured the user can say "take picture". To prove that the picture has been taken and stored the user will receive an haptic feedback (vibration) on the primary hand controller. 

Create/modify/save a mask 
^^^^^^^^^^^^^^^^^^^^^^^^^
iDaVIE-v allows to create a mask or to modify an existing mask in VR. Both can be done using the "Paint menu" that can be invoked from the "Quick menu" by lasering the brush icon. Using the functionality available in the "Paint menu" the user can add or delete mask voxels using the controllers. Once done the user can save the created/updated mask overwriting an existing one or creating a new one. As also explained in :ref:`inputs_outputs`:

* if a mask is loaded and modified in VR then it can be saved either overwriting the original mask **or**  as a copy. In the former case the mask will be saved with the same name of the original mask and in the same directory, in the latter case the suffix :literal:`-copy.fits` will be added to the original mask name and the edited mask will be saved in the same directory as the original mask (e.g. the edited mask file name will then be :literal:`originalmaskname-copy.fits`).
* if no mask is provided in input, but one is created in iDaVIE-v, then the created mask is saved in the same directory of the data cube and a suffix :literal:`-mask.fits` will be addedd to the cube name to indicate the maks file (e.g. the created mask file name will then be :literal:`originalcubename-mask.fits`).

**Demo TBD**

Interact with catalogs in VR
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
iDaVIE-v allows to load catalos from the Desktop GUI and to overplot them on the visualised data cube.

.. raw:: html

    <video controls loop style="width:100%;height:auto;">
      <source src="_static/Demo-catalogue-allthree.mp4" type="video/mp4">
    </video>

Create stats and save moment maps
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
iDaVIE-v allows to investigate basic stats of the cube and to create both moment 0 and moment 1 of a data cube. The user can create the moment maps for the entire cube or for a single selected region. In case a mask is available the moment maps thresholds are set by the mask, but they can be changed manually. If no mask is available then the thresholds should be set manually using the options available in the moment map windows. The moment maps can then be saved as png.

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




