<div>**FIRST SETUP**</div>

*   Install java jdk
*   Install node.js
*   Install Python 2.x
*   Install Android studio

<div>Install react-native with node from cmd. Command:</div>

<div>

<div>npm install -g react-native-cli</div>

</div>

<div>If npm is not recognised just add</div>

<div>

<div>

<div>;C:\Program Files\nodejs\</div>

</div>

</div>

<div>To the end of your Path variable on the "User variable" section of the Environment Variables on the System Properties.</div>

<div>Create a projects folder like /reactnative where do you like ( es: _C:\Users\Andrea\Documents\reactnative )_</div>

<div>Go into the /reactnative folder and generate a new project called with react from cmd, command:</div>

<div>

<div>react-native init albums</div>

</div>

<div>Open Android Studio and select _open a new existing Android studio project  _and select the /android folder into the "albums" project created above (example: _C:\Users\Andrea\Documents\reactnative\albums\android )_</div>

<div>Android studio could output an error about "missing platforms", click on the link in the error and install all the missing sdk</div>

<div>Next go in the AVD manager and create an android emulator for debug  (note it work only with Intel CPU, with amd you need to debug on a real device connected with usb debug mode)</div>

<div>At today react-native use API 23 Marshmallow, select them (and eventually dowload if needed)</div>

<div>To complete the react-native installation need to add a windows environment user variables (if not already present) about jdk installation path and a new path in the variable "PATH":</div>

<div>**new variable:**</div>

<div>name: JAVA_HOME</div>

<div>value:  C:\Program Files\Java\jdk1.8.0_111</div>

<div>**path to add**</div>

<div>;C:\Users\Andrea\AppData\Local\Android\sdk\platform-tools</div>

<div>Then close and reopen cmd to have the modification take effect, go into /reactnative/albums and run the command:</div>

<div>

<div>

<div>_react-native run-android_</div>

</div>

</div>

<div>This will start the react-native package (on antoher window), it will take care of take all the javascript code and compress into a single javascript file and make it available to the device.</div>

<div>In the original window the application will build for android and it will be automatically installed and opened on the device.</div>

<div>**issue about slow and unresponsive android virtual emulator**</div>

<div>A good alternative to the original emulator is the free version of [genymotion emulator](https://www.genymotion.com/fun-zone/) , it's faster and should work also on AMD machines.</div>

*   install genymotion emulator
*   install genymotion plugin in android studio file->settings->plugin->browse repositories and search for genymotion
*   go into genymotion (standalone) settings and in the ADB panel select "use custom android sdk tools". The path on windows 10 is usually in  _C:\Users\Andrea\AppData\Local\Android\sdk_
