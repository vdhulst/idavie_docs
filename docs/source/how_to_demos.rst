.. _how_to_demos:

"How to" demos
==============

.. note:: This section is under construction. Some elements in the ideos may slightly differ from what the user actually see in the rendering of the current software. We apologies for the inconvenience.

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
TBD

Interact with catalogs in VR
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. raw:: html

    <video controls loop style="width:100%;height:auto;">
      <source src="_static/Demo-catalogue-allthree.mp4" type="video/mp4">
    </video>

Create stats and save moment maps
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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




