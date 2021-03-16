.. _inputs_outputs:

Input & Outputs
===============
In this section we describe what kind of file format can be ingested in iDaVIE-v and what file and in which formats are saved as data product of iDaVIE-v.

Inputs
------
Standard Real*4 (32-bit) FITS cubes for both the data and the (optional) mask.  There should be three axis, as defined by NAXIS1, NAXIS2 and NAXIS3 in the header.  Avoid using the NAXIS4 as the third dimension, it is ignored by the software. Multiple catalogs can also be loaded if in VOTable format.

Outputs
-------
iDaVIE-v provides:

* **PNG** files of screenshots and moment maps stored in :literal:`Output/Camera` 
* **VOTable** catalog originated by an edited or created mask stored in :literal:`Output/Catalogs`
* **FITS** file of created/modified mask:

  * if a mask is loaded and modified in VR then it can be saved either overwriting the original mask **or**  as a copy. In the former case the mask will be saved with the same name of the original mask and in the same directory, in the latter case the suffix :literal:`-copy.fits` will be added to the original mask name and the edited mask will be saved in the same directory as the original mask (e.g. the edited mask file name will then be :literal:`originalmaskname-copy.fits`).
  * if no mask is provided in input, but one is created in iDaVIE-v, then the created mask is saved in the same directory of the data cube and a suffix :literal:`-mask.fits` will be addedd to the cube name to indicate the maks file (e.g. the created mask file name will then be :literal:`originalcubename-mask.fits`).
