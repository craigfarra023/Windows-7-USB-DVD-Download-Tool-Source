the source from http://go.microsoft.com/fwlink/?LinkId=218888
or https://www.microsoft.com/en-us/download/confirmation.aspx?id=56485&6B49FDFB-8E5B-4B07-BC31-15695C5A2143=1
or https://download.microsoft.com/download/C/4/8/C48F6E20-FE20-41C6-8C1C-408FE7B49A3A/Windows7-USB-DVD-Download-Tool-Installer-en-US.exe



<br/>
<br/>
<hr/>
<br/>

For more information about the Windows 7 USB/DVD Download Tool, please see 
http://store.microsoft.com/help/ISO-Tool. 


The Windows 7 USD/DVD Download Tool uses material from ImageMaster, a .NET C#
application for reading and writing disc images (*.iso files).  ImageMaster 
is licensed under the terms of the GPL.  For more information about ImageMaster,
please see http://imagemaster.codeplex.com/.


This project uses the WIX Votive plugin for Visual Studio 2008.  Please see
http://wix.sourceforge.net/votive.html for installation instructions.


To build in Visual Studio 2008:

1. Make desired changes to the source code.

2. Copy the wudtsource.zip file to the same directory as the .sln file.

3. Build the project in Visual Studio.


To create localized installers and self-extracting files:

1. Build the project as described above.

2. Run the Install\CreateLocalizedInstallers.cmd script to create the 
   localized MSI installers.


To bypass formatting the USB device within the tool:

1. Ensure the registry key "HKCU\SOFTWARE\Microsoft\ISO Backup Tool" is created.

2. Create a new DWORD value named "DisableFormat" in this location and set the value to 1.

NOTE: The USB device should be formatted manually before running the tool.