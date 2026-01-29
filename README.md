# PDP1-DPY
A Type 30 display for the PiDP1 project<br><br>
This app is an optional update for the PiDP1 to create a Type 30 display.<br>
The repo contains a build system for both Linux and Windows (Visual Studio .. not VSCode).<br>
Both apps are cut down builds from Simh.<br>
The special feature is the the app can be run on a remote machine. It will connect to a PiDP1 instance as follows.<br>
On the PiDP1 machine, start the PiDP1 app in 'apps' mode (see the instruction manual for this).<br>
Windows:<br>
You will then need to close the P7 Sim window. Under windows, run the pdp1_dpy solution from visual studio.<br>
The solution file is in the ./Visual Studio Projects directory.<br>
The app requires SDL3. This is included in the windows build directory.
At the simh prompt, type 'set dpy ena' and then att dpy <name of your PiDP1 machine> and the display should start.<br>
The app window is 2014x1069 so you need a sizeable display on the windows machine.<br>
Raspbian:<br>
You may build and run the app either on the PiDP1 machine or another Pi on the same network.<br>
However, here is the tricky bit. SDL3 development files and libraries are not available on Raspbian (as yet).


