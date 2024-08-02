.. _inputs_outputs:

Input & Outputs
===============
In this section we describe what kinds of file can be ingested by iDaVIE and what files and formats are saved as data products of iDaVIE.

Inputs
------
Standard Real*4 (32-bit) FITS cubes for both the data and the (optional) mask.  There should be three axes, as defined by NAXIS1, NAXIS2, and NAXIS3 in the header. If the third visual dimension is in NAXIS4 (e.g., some ASKAPP cubes), the user can choose which axis to use as the third (*z*) dimension. Multiple catalogs can also be loaded if in VOTable format.

Outputs
-------
iDaVIE provides:

* **PNG** Screenshots and moment maps exported as PNG files, stored in :literal:`Output/Camera` and :literal:`Output/MomentMaps` respectively.
* **VOTable** Catalog exported from an edited or created mask, stored in :literal:`Output/Catalogs`.
* **log** Debug files created by iDaVIE, stored in :literal:`Output/Logs`. Used for error reporting and should be attached when reporting issues.
* **FITS** Created or modified masks, or moment maps exported as FITS files:

  * If a mask is loaded and modified in VR then it can be saved either overwriting the original mask **or**  as a copy. In the former case the mask will be saved with the same name of the original mask and in the same directory, in the latter case the suffix :literal:`-copy.fits` will be added to the original mask name and the edited mask will be saved in the same directory as the original mask (e.g. the edited mask file name will then be :literal:`originalmaskname-copy.fits`).
  * If no mask is provided in input, but one is created in iDaVIE, then the created mask is saved in the same directory of the data cube and a suffix :literal:`-mask.fits` will be addedd to the cube name to indicate the maks file (e.g. the created mask file name will then be :literal:`originalcubename-mask.fits`).
  * Moment maps are saved to :literal:`Output/MomentMaps/Moment_map_[0/1]_yyyyMMdd_Hmmss.png`, where :literal:`yyyyMMdd_Hmmss` is the timestamp when the files are saved.
