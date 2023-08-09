# Passthrough-Demo
Starter project for Standalone and PCVR passthrough with Meta headsets

![hippo](https://j.gifs.com/46rgO7.gif)

**Setup instructions:**
1. With a Quest, Quest 2 or Quest Pro, launch PC with either quest link or air link from inside the headset

2. In the Oculus Desktop App, go to Settings > Beta > Emable the two following toggles:
- Developer Runtime Features
- Passthrough over Oculus Link

3. After cloning the project, download the latest compatible MetaXR plugin. The default unreal version for this project is 5.1.1, so the most recent compatible MetaXR plugin should be here: https://developer.oculus.com/downloads/package/unreal-engine-5-integration/54.0

4. Unzip the MetaXR file and put the extracted folder into Github > Passthrough-Demo > Plugins (Replace any metaXR files already there)

5. After copying over the meta plugin, open the .uproject

6. Select play in VR mode, the level should open with passthrough active.


**Controls:**

- Move: Right Joystick

- Snap Turn: Left Joystick

- Return to Center: X

- Toggle Passthrough: Y

- Grab: Oculus Grips

- Scale grabbed plane: Right joystick X and Y axis



**TroubleShooting:**
If passthrough is not working in editor, try these steps in order:
1. Ensure the latest MetaXR plugin is installed (see setup instructions above)
2. Ensure Link Passthrough over Link is enabled in the Desktop Oculus App (Settings > Beta),
3. Close the Unreal Editor and restart OVRService (Task Manager > Services > OVRService)
4. Re-open the project and try playing again

There is a known bug where Passthrough can stop working after the headset goes to sleep while the editor is open. Restarting OVRservice and re-opening the project should solve this bug whenever it happens
