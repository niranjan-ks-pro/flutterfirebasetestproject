# flutterfirebasetestproject

Flutter Firebase Analytics integration for flutter App. July2023
Create empty project in VS Code.
Create Firebase Project in Firebase Console.
Install firebase CLI and Flutter SDK if does not present in your PC.
Install and run Firebase CLI
dart pub global activate flutterfire_cli
Skipping the above warning → Warning: Pub installs executables into C:\Users\niran\AppData\Local\Pub\Cache\bin, which is not on your path.
You can fix that by adding that directory to your system's "Path" environment variable.
A web search for "configure windows path" will show you how.
ignoring this error now!

Run Command in your project directory →flutter pub add firebase_core
Enable Developer Options in Windows
Run Command in your project directory → flutterfire configure - project=flutterfirebasetestproject1
Creates a new file (below)automatically in your flutter project.
initialize firebase and plugins. (Skipping this step for now)
Adding this in main.dart as per Add Firebase to your Flutter app (google.com)
Verify the firebase_core is present in pub_spec.yaml
Add Firebase plugins https://firebase.google.com/docs/flutter/setup?platform=android#add-plugins
flutter pub add PLUGIN_NAME
Enable debug vire as per link Add Firebase to your Flutter app (google.com) point number 5.b.
_________________________________________________
Enable ADB mode
Step 1 : enable USB/Wifi debugging in mobile device.
Step 2 : Download platform-tools from link https://dl.google.com/android/repository/platform-tools-latest-windows.zip
Set env variable
__________________________________________________
open cmd/powershell in platform-tools's location.
Run adb devices command.
Run adb shell setprop debug.firebase.analytics.app PACKAGE_NAME command.
Now Click on the running application on the mobile to create any event.
Then go to firebase.console → Analytics Dashboard to see the user activity.


https://medium.com/p/f354189e907
