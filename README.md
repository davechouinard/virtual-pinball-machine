virtual-pinball-machine
=======================

Notes for building a virtual pinball machine running under the Windows 8 operating system.

### Software

**Visual Pinball**

Visual Pinball is a free (for non-commercial use) pinball game engine and editor.  There is a nice community at vpforums.org writing tables and helping support this engine.

Follow the VP installer guide for installation using the VPInstaller 1.0.3:

http://www.vpforums.org/index.php?app=tutorials&article=1

When updating to vpinball991 in Windows 8 you may encounter this error:
>The program can't start bceause d3dx9_43.dll is missing from your computer.

This is fixed by installing the DirectX End-User Runtime:

http://www.microsoft.com/en-us/download/details.aspx?id=35

After hooking up a 1080p TV and looking at Preferences->Video Options I noticed that 1920x1080 was not in the list of resolutions.  This is apparently because of a Windows 7/8 scaling issue.  To fix set everything to 'smaller'.

http://windows.microsoft.com/en-us/windows7/make-the-text-on-your-screen-larger-or-smaller?v=t

**PinballX**

PinballX is a pinball menu front end for users to select tables.

http://www.pinballx.net

Make sure to right click the icon and go into the properties and make sure 'run as administrator' is selected.

**DirectB2S**

DirectB2S is an animated backglass server.  It is also a requirement for Direct Output Framework to drive LED boards etc.

Download the zip and follow the install instructions.

http://www.vpforums.org/index.php?app=tutorials&article=136

**Direct Output Framework**

Direct Output Framework is a way to control LED boards and other hardware.  It works through the DirectB2S plugin interface.

Download and install according to:

http://directoutput.github.io/DirectOutput/

Generate *directoutputconfig20.ini* file for pacled64 support.  

That file can be generated here: http://configtool.vpuniverse.com/

Place *directoutputconfig20.ini* inside the tables folder.



### Hardware
**I-PAC**

The I-PAC is an input controller board and lets you connect arcade buttons, switches etc. to your PC through a USB interface.  It basically acts like a keyboard and sends a certain keystroke when a button is pressed.

http://www.ultimarc.com/ipac1.html


**PacLED64**

The PacLED64 is an LED controller board and lets you connect LED lights.  The lights can be programmed in many different ways to interact with the game software so that lights activate at the correct times etc.

http://www.ultimarc.com/pacled64.html

Many people use an alternate board called LED-Wiz to control many different types of outputs such as solenoids, motors, lights etc. but for my simple set of LED buttons the PacLED64 seemed a simpler more purpose built solution.

**Flipper Buttons and Leaf Switches**

The flipper buttons and leaf switches that drive the virtual pinball flippers can be obtained here and are known to work well in a low voltage I-PAC like setup.

I decided to put 4 of these into my cabinet.  Two act as the main flipper buttons and two act as nudge buttons.  I connect these to the arrow key inputs on the I-PAC so that I can use them to navigate up/down, left/right in alternate game engines such as pinball fx2 or the pinball arcade which have their own in-game menu interfaces.

http://virtuapin.net/index.php?main_page=index&cPath=26


### Cabinet
This section will cover building a pinball cabinet out of plywood.
