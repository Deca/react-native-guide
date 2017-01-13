**FIRST SETUP**

-   Install java jdk
-   Install node.js
-   Install Python 2.x
-   Install Android studio

Install react-native with node from cmd. Command:

npm install -g react-native-cli

If npm is not recognised just add

;C:\\Program Files\\nodejs\\

To the end of your Path variable on the “User variable” section of the Environment Variables on the System Properties.

Create a projects folder like /reactnative where do you like ( es: *C:\\Users\\Andrea\\Documents\\reactnative )*

* *

Go into the /reactnative folder and generate a new project called with react from cmd, command:

react-native init albums

Open Android Studio and select *open a new existing Android studio project  *and select the /android folder into the “albums” project created above (example: *C:\\Users\\Andrea\\Documents\\reactnative\\albums\\android )*

* *

Android studio could output an error about “missing platforms”, click on the link in the error and install all the missing sdk

Next go in the AVD manager and create an android emulator for debug  (note it work only with Intel CPU, with amd you need to debug on a real device connected with usb debug mode)

At today react-native use API 23 Marshmallow, select them (and eventually dowload if needed)

To complete the react-native installation need to add a windows environment user variables (if not already present) about jdk installation path and a new path in the variable “PATH”:

** **

**new variable:**

name: JAVA\_HOME

value:  C:\\Program Files\\Java\\jdk1.8.0\_111

**path to add**

;C:\\Users\\Andrea\\AppData\\Local\\Android\\sdk\\platform-tools

Then close and reopen cmd to have the modification take effect, go into /reactnative/albums and run the command:

*react-native run-android*

This will start the react-native package (on antoher window), it will take care of take all the javascript code and compress into a single javascript file and make it available to the device.

In the original window the application will build for android and it will be automatically installed and opened on the device.

**issue about slow and unresponsive android virtual emulator**

A good alternative to the original emulator is the free version of [genymotion emulator] , it’s faster and should work also on AMD machines.
 
- install genymotion emulator
- install genymotion plugin in android studio file->settings->plugin->browse repositories and search for genymotion
- go into genymotion (standalone) settings and in the ADB panel select "use custom android sdk tools". The path on windows 10 is usually in  C:\Users\Andrea\AppData\Local\Android\sdk

  [genymotion emulator]: https://www.genymotion.com/fun-zone/
