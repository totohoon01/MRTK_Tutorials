# MRTK Tutorials

## Basic Settings

1. Create Project with 2019 / <b>2020 LTS</b>
2. Open Build Settings,
   - <b>Universal Windows</b> Platform
   - <b>Target Device</b> : Hololens
   - <b>Architecture</b> : ARM64
   - <b>Build and Run On</b> : USB Device
     Switch Platform
3. Get 'MRTK Feature Tool' [Download](https://www.microsoft.com/en-us/download/details.aspx?id=102778)
4. Execute 'MixedRealityFeatureTool.exe', Open Project Path
5. Add Features
   - <b>Mixed Reality Toolkit Foundation</b>
   - <b>Mixed Reality OpenXR Plugin</b>
6. <b>RESTART UNITY</b>
7. MRTK Settings(auto poped)
   - Unity OpenXR Plugin(Recommended)
   - Show XR Plug-in Management Settings
   - Check <b>'OpenXR'</b>
   - Apply Settings
   - Next(Ignore the error)
   - Apply
8. Project Settings->Player->Publishing Settings->Package name = MRTK-Tutorials

## SceneSample

1. Mixed Reality -> Toolkit -> Add to Scene and Configure
2. Add Object('cude'), Add script **NearInteractionGrabble, Object Manipulator**
3. QEWASD == Moving, Space/LShift == RL

## Build

1. Build on Unity
2. Open **.sln** in **Visual Studio**
3. **Relseae, ARM64**
4. Start without Debugging
5. Bulid -> Publich app
