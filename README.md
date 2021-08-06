# MRTK Tutorials

## Settings

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

## Build

1. Build on Unity
2. Open **.sln** in **Visual Studio**
3. **Relseae, ARM64**
4. Start without Debugging
5. Bulid -> Publish app

<hr>

### Scene Settings & Manipulating Object

1. Mixed Reality -> Toolkit -> Add to Scene and Configure
2. Add Object('cude'), Add script **NearInteractionGrabble, Object Manipulator**
3. QEWASD == Moving, Space/LShift == RL

### Creating Custom Profile

1. In **"MixedRealityToolkit"** Object, **DefaultHoloLens2ConfigurationProfile** -> clone
2. In custom profile, select **'Spatial Awareness'**
3. Check Enable, Clone Default profile.
4. **XR SDK Windows Mixed Reality Spatial Mesh Observer** -> clone
5. Display Settings -> Occulsion, 인식은 하되 표시를 안함. 필요없으면 공간인식을 꺼두는게 성능향상

### Rover Examples

1. Model 구성
2. RoverParts에 **GridObjectCollection** 추가
   - 정렬 유형: 사전순
   - 레이아웃: 수평
   - 셀 너비: 0.25
   - 부모에서의 거리: 0.38
   - Update Collection
   - 오브젝트 정렬용??
3. **Packages > Mixed Reality Toolkit Foundation > SDK > Features > Utilities > Solvers**
   - Solver : 오브젝트가 사용자 / 다른 오브젝트를 따라다니게 설정 스크립트
4. Chevron프리팹(0,0,2) -> Directional Indicator 추가
