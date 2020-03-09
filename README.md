# STT-Hololens

Unity translation app using Google Cloud Speech-to-Text on Hololens

## Developement environment

### Tools

- Unity 2019.3.4f1
  - Add modules `Universal Windows Platform Build Support`, 2.1GB
  - Pacakges
    - Windows Mixed Reality 4.2.1
- Visual Studio Community 2019 16.4.5
  - Add workloads `Game development with Unity` (Unity)
  - Add workloads `Desktop development with C++` (UWP)
  - Add workloads `Universal Windows Platform development` (UWP)

### Device

- Hololens OS build 10.0.17763.1039

## Build UWP project in Unity

- Open Unity project scene from Assets/Scenes/STT_Hololens.scene
- Open Build Settigs popup `Ctrl+Shift+B` or `File > BuildSettings...`
- Checkout build options
  - ![UnityBuildSettings.png](UnityBuildSettings.png)
- Click `Build` button
- Select exist folder to UWP project target.

## Build Hololens app in UWP project

- Open Visual Studio Solution file from <`BuildFromUnityFolder`>/STT-Hololens.sln
- Checkout build options
  - ![VisualStudioBuildSettings.png](VisualStudioBuildSettings.png)
  - Solution configurations: Release or Master
  - Solution platforms: x86
  - Build to target: Device(hololens)
- Click Deivce(Debug run) button