<div><b>FIRST SETUP</b></div>
<ul>
 	<li>Install java jdk</li>
 	<li>Install node.js</li>
 	<li>Install Python 2.x</li>
 	<li>Install Android studio</li>
</ul>
<div>Install react-native with node from cmd. Command:</div>
<div>
<div>npm install -g react-native-cli</div>
</div>
<div></div>
<div>If npm is not recognised just add</div>
<div>
<div>
<div>;C:\Program Files\nodejs\</div>
</div>
</div>
<div>To the end of your Path variable on the "User variable" section of the Environment Variables on the System Properties.</div>
<div></div>
<div>Create a projects folder like /reactnative where do you like ( es: <i>C:\Users\Andrea\Documents\reactnative )</i></div>
<div><i> </i></div>
<div>Go into the /reactnative folder and generate a new project called with react from cmd, command:</div>
<div>
<div>react-native init albums</div>
</div>
<div></div>
<div>Open Android Studio and select <i>open a new existing Android studio project  </i>and select the /android folder into the "albums" project created above (example: <i>C:\Users\Andrea\Documents\reactnative\albums\android )</i></div>
<div><i> </i></div>
<div>Android studio could output an error about "missing platforms", click on the link in the error and install all the missing sdk</div>
<div></div>
<div>Next go in the AVD manager and create an android emulator for debug  (note it work only with Intel CPU, with amd you need to debug on a real device connected with usb debug mode)</div>
<div>At today react-native use API 23 Marshmallow, select them (and eventually dowload if needed)</div>
<div></div>
<div>To complete the react-native installation need to add a windows environment user variables (if not already present) about jdk installation path and a new path in the variable "PATH":</div>
<div><b> </b></div>
<div></div>
<div><b>new variable:</b></div>
<div>name: JAVA_HOME</div>
<div>value:  C:\Program Files\Java\jdk1.8.0_111</div>
<div></div>
<div></div>
<div><b>path to add</b></div>
<div>;C:\Users\Andrea\AppData\Local\Android\sdk\platform-tools</div>
<div></div>
<div>Then close and reopen cmd to have the modification take effect, go into /reactnative/albums and run the command:</div>
<div></div>
<div>
<div>
<div><em>react-native run-android</em></div>
</div>
</div>
<div></div>
<div>This will start the react-native package (on antoher window), it will take care of take all the javascript code and compress into a single javascript file and make it available to the device.</div>
<div>In the original window the application will build for android and it will be automatically installed and opened on the device.</div>
<div></div>
<div></div>
<div><b>issue about slow and unresponsive android virtual emulator</b></div>
<div>A good alternative to the original emulator is the free version of <a href="https://www.genymotion.com/fun-zone/">genymotion emulator</a> , it's faster and should work also on AMD machines.</div>
<ul>
 	<li>install genymotion emulator</li>
 	<li>install genymotion plugin in android studio file-&gt;settings-&gt;plugin-&gt;browse repositories and search for genymotion</li>
 	<li>go into genymotion (standalone) settings and in the ADB panel select "use custom android sdk tools". The path on windows 10 is usually in  <i>C:\Users\Andrea\AppData\Local\Android\sdk</i></li>
</ul>
<div></div>
<div></div>
