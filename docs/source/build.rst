.. _build:
Building i-DaVIE-v from source
==============================

As a Unity project, there are several steps to follow to compile i-DaVIE-v from source.

Unfortunately, due to the limitations on VR headset drivers on Unix operating systems, we can only support Windows at the moment. We keep a close eye on developments in the VR space and will support Unix as soon as it becomes feasible.
Prerequisites
-------------
#. Install Unity
    * Download `Unity Hub for Windows <https://public-cdn.cloud.unity3d.com/hub/prod/UnityHubSetup.exe>` from Unity's website and install it.
    * From the Unity Hub, install Unity version 2021.3.xf1, where x is the highest number available.

#. Install CMake
    * Download `CMake for Windows <https://cmake.org/download/>` and install it.
    * Make sure you can run :literal:`cmake` from the PowerShell terminal (or command line).
        - `cmake --version` is a good test.

#. Install vcpkg
    * Download `vcpkg <https://github.com/microsoft/vcpkg>` and install it.
    * Make sure to note the path to the vcpkg root folder, found at :literal:`C:\vcpkg` for default installations.

#. Download i-DaVIE-v source code
    * Download the i-DaVIE-v source code from the `GitHub repository <https://github.com/idia-astro/idia_unity_vr>`.
    * (Optional) You can do this through a Git client, such as `GitHub Desktop <https://desktop.github.com/download/>` or `Git Extensions <https://github.com/gitextensions/gitextensions/releases/latest>`.

#. Run the configuration script
    * Open a PowerShell terminal in the i-DaVIE-v root folder
    * Run the :literal:`configure.ps1` script. This script takes two arguments: the vcpkg root folder, and the Unity executable. The default assumption is positional arguments.
    * For example: :literal:`.\configure.ps1 "C:\vcpkg" "C:\Program Files\Unity\2021.3.xf1\Editor\Unity.exe"`
    * (Optional) You can specify the vcpkg root with the :literal:`-v` or :literal:`-vcpkg` flags.
    * (Optional) You can specify the Unity executable with :literal:`-u` or :literal:`-unity` flags.
    * (Optional) For example: :literal:`.\configure.ps1 -v "C:\vcpkg" -u "C:\Program Files\Unity\2021.3.xf1\Editor\Unity.exe"`
  
#. Generate SteamVR actions
    * Open i-DaVIE-v in the Unity Editor.
    * Under **Window->SteamVR Input**, click the **Save and generate** button.
  
#. Build i-DaVIE-v
    * Open i-DaVIE-v in the Unity Editor.
    * Open the build settings menu under **File->Build Settings**.
    * Click on the Player Settings button on the bottom left.
    * Under XR Plug-in Management (scroll down on the left), make sure that OpenVR Loader is selected in the list of Plug-in Providers.
    * Click the **Build** button and select your destination folder.