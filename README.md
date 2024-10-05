# Mocap Animation 

Mocap Animation is a package that uses OpenXR’s tracking APIs to expose Meta Quest Pro’s Body Tracking (BT), Eye Tracking (ET), and Face Tracking (FT) capabilities.
With this package, developers can leverage tracking to populate VR environments with custom avatars that bring the expressiveness of users into the virtual environments that they create.

## How to Use

### Load the project

### Launch the project in the Unreal Editor using one of the following options.

#### Epic Games Launcher with MetaXR plugin

The easiest way to get started is to use the prebuilt Unreal Engine from the Epic Games Launcher, with MetaXR plugin.

1. Install the [Epic Games Launcher](https://www.epicgames.com/store/en-US/download)
2. In the launcher, install UE5 (recommended).
3. Download and install the MetaXR plugin from the [Unreal Engine 5 Integration download page](https://developer.oculus.com/downloads/package/unreal-engine-5-integration).
4. Launch the Unreal Editor
5. From "Recent Projects", click "Browse" and select `MovementSample.uproject`

#### Oculus Unreal fork

The Oculus Unreal fork will give you the most up to date integration of Oculus features. However, you must build the editor from its source.

Follow the instructions on [Accessing Unreal Engine source code on GitHub](https://www.unrealengine.com/en-US/ue-on-github) to obtain:
- an Epic account
- a GitHub account
- authorization to access the Unreal Engine source repository
Disregard instructions on downloading Epic’s Unreal Engine source code as you will be building the Oculus-VR fork of Unreal Engine source.

Make sure you have Visual Studio installed properly:
- Launch the Visual Studio Installer and click Modify for the Visual Studio version you want to use.
- Under the Workloads tab, click Game development with C++ if it isn’t checked and then click Modify.

1. Download the source code from the [Oculus-VR fork of Unreal Engine on GitHub](https://github.com/Oculus-VR/UnrealEngine).
2. Open a command prompt in the root of the Unreal, then run this command:
```sh
.\GenerateProjectFiles.bat -Game MovementSample -Engine <full path to Unreal-MovementSample directory>\MovementSample.uproject
```
3. Open the `MovementSample.sln` file that has been generated in the `Unreal-MovementSample` directory.
4. Set `MovementSample` as the start-up project and `Development Editor` as the configuration.
5. Hit `F5` to build and debug the project (and the engine).
    - Depending on your machine, the build may take awhile to complete.

#### Some result were captured with:
1. face capturing with lipsync

<img src='imgs/face capture_lipsync.gif' align="left" width=1024>
&nbsp;

2. Upper motion capturing recorded 

<img src='imgs/UpperBoady_motionCapture.gif' align="left" width=1024>
&nbsp;

# Licenses
The Unreal-Movement is released under the [Oculus SDK License](https://github.com/oculus-samples/Unreal-Movement/blob/main/LICENSE). The MIT License applies to only certain, clearly marked documents. If an individual file does not indicate which license it is subject to, then the Oculus License applies.
