## Flutter - Dev Notes

### Starting the Android emulator from CLI

Use the following commands to start the Android emulator (one of your AVD devices) from the command line, without having to start Android Studio:

```bash
$ ~/Library/Android/sdk/tools/bin/avdmanager list avd        // To list the existing virtual devices.
$ ~/Library/Android/sdk/tools/emulator -avd Nexus_5_API_27   // Start the device having that name.
```
**Note:** It's way easier to start it from VSCode: When starting the Debug (F5), it asks you which device to use if none is detected (shown in the right side of the status bar).

<br/>

### VSCode settings

Additional Dart and Flutter related settings in VSCode were defined. See the details [here](../_IDEs/vscode/readme.md).

<br/>

### Cleanup CoreSimulator storage

As `~/Library/Developer/CoreSimulator/Devices` tends to grow considerably over time, a quick option to do cleanup is to run `xcrun simctl delete unavailable` from command line.

<br/>

