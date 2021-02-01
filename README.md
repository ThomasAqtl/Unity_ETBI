# Unity_ETBI
Unity_ETBI (Eye-Tracking Based Interactions) is a school project in which I explore gaze-based interactions in VR with Unity.

## Prerequisites
Prefabs and scripts has been made to work in Unity version 2018.3.14f1. The VR headset used is the HTC Vive Pro Eye. External packages are needed and are detailed further.

## How to use

1. Install Unity. I recommend 2018.3.14f1 version to ensure everything works fine. Then creates a new empty 3D projetc.
2. Follow [Tobii's guide](https://vr.tobii.com/sdk/develop/unity/getting-started/vive-pro-eye/) to set your project with needed packages.
3. Import this repo's packages into your project.

## Contents
### Scene
The *AllInOne* scene is a simple scene with two tables and objects to interact with. Pick the interaction mode of your choice directly from the inspector.

### Scripts
- *InteractionManager.cs* handles which interaction user wants to use. Attach it to a player object and pick options in from the inspector.
- *GazeTakeable.cs* must be attached to any object that needs to receive focus.

#### Controller
- *GazeTake.cs* handles controller-based interactions.

#### Eye wink
- *EyeManager.cs* handles potential unstability in eye tracking.
- *WinkToTake.cs* handles wink-based interactions.
- *LongBlinkResetPosition.cs* triggers object position reset by long blinking (usefull when debugging)

#### Voice command
- *VoiceManager.cs* handles voice input and keywords.
- *VoiceToTake.cs* handles voice-command-based interactions.

#### Spot
- *SpotGazeTarget* manages spots : outline when focused, available or not.

### Prefabs
In this folder you will find following prefabs :
- sphere and cube from *AllInOne* scene
- spots

These can be used in any other scene.
