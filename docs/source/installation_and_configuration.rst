.. _installation_configuration:

Installation and configuration
==============================
.. note:: The software is in active development, and while we do our best to ensure that there are no issues present, there might be some. We welcome bug reports and feature requests on the GitHub `repository <https://github.com/idia-astro/iDaVIE/>`_. 

Executable
-----------
Once the requirements described in :ref:`requirements`, are installed and working correctly, the user can download and unzip the provided :literal:`iDaVIE_v.1.0.zip`, which contains the executable .exe (and other reference files). The zip file is available on Github at this `link <https://github.com/idia-astro/iDaVIE/releases>`_.

.. raw:: html

    <img src="_static/idavie-pkg-edit.png"
         style="width:100%;height:auto;">

To start the software, double-click on the executable iDaVIE file.
 

Source code
-----------
Please see :ref:`build` for instructions on building iDaVIE from the source code. We also provide detailed :ref:`contribution` guidelines.

Troubleshooting
---------------
In this section we share some useful tips where we found a solution to a known issue:

- Under some circumstances, the voice commands stop working. If this happens, we found that the following sequence of actions usually solves the problem (**NOTE**: this solution has been tested only with Oculus Rift S and on machines where the RealTek Audio driver is installed, we cannot assure it will work for all configurations)

  #. take the headset off 
  
  #. make sure the iDaVIE Desktop GUI is front and center and no other windows are in front of it
  
  #. use the Windows search function (lower left hand corner - says Type here to search), and type audio
  
  #. open the RealTek Audio Console that will apper after the search
  
  #. check that the Microphone is set to maxium;   toggle <mute> on and then off. Now the mic should be on and ready to receive commands.

  #. close the Audio Console

  #. put the headset back on and use the voice commands as normal.

- If errors are encountered that you can't solve, please:

  #. Post an issue on the Github repository, or,
  
  #. Make contact with us and send us the log files along with your bug reports. The log files can be found in the directory :literal:`i-DaVIE/Outputs/Logs`.
  
.. WARNING:: Unity only allows for a maximum of two log files to be stored. Therefore, if a problem is encountered with iDaVIE, make sure to copy the log file to a different folder **BEFORE** starting a new iDaVIE session, otherwise the log file reporting the specific problem encountered will be lost.

Known issues
------------
The following are issues we already know about and that will be fixed as soon as possible:

#. Problem with virus protection systems. We will make a request to Norton to have our software "whitelisted". In the meantime the virus protection does not recognize the .exe and puts up the warning. See more details `here <https://www.symantec.com/connect/forums/how-avoid-wsreputation1-error>`_
