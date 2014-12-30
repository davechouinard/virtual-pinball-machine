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

**DirectB2S**

DirectB2S is an animated backglass engine.  It is also a requirement for Direct Output Framework to drive LED boards etc.

Download the zip and follow the install instructions.

http://www.vpforums.org/index.php?app=tutorials&article=136

**PinballX**

PinballX is a pinball menu front end for users to select tables.

http://www.pinballx.net

Make sure to right click the icon and go into the properties and make sure 'run as administrator' is selected.

**Direct Output Framework**

Direct Output Framework is a new way to control LED boards and other hardware.

Download and install according to:

http://directoutput.github.io/DirectOutput/

Generate *directoutputconfig20.ini* file for pacled64 support.  

That file can be generated here: http://configtool.vpuniverse.com/

Place *directoutputconfig20.ini* inside the tables folder.



### Hardware
This section will cover the various hardware related to setting up a virtual pinball machine.

### Cabinet
This section will cover building a pinball cabinet out of plywood.
