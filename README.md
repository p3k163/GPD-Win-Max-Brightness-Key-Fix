# GPD-Win-Max-Brightness-Key-Fix

This repository includes patches for the brightness control key on GPD Win Max.

A modified version of VoodooPS2 is included, the repository of VoodooPS2 is https://github.com/acidanthera/VoodooPS2.

VoodooPS2 comes together with APPLE PUBLIC SOURCE LICENSE, please read the license before download the modified version in this repository, thanks.

It is quite easy to fix the brightness control key for GPD Win Max.

Step 0: Make sure the graphics card is recognized and the brightness can be controlled in system preferences.

Step 1: Download SSDT-BRNK.aml, hotpatch.plist and prepare your config.plist.

Step 2: Move SSDT-BRNK.aml to your patched ACPI folder.

Step 3: Add SSDT-BRNK.aml to your config.plist, add two patches for DSDT to your config.plist, if you are using opencore bootloader, the template is ready for copy and paste, please check the hotpatch.plist for more details, if you are using clover bootloader, you can add patches manually, open hotpatch.plist, copy and paste the data that clover requires, then you are ready to have a try.

Step 4: Press Fn+F4/F5 to test whether the brightness control works.

Step 5: For a better experience, you can download the VoodooPS2 in this repository, replace your VoodooPS2 with this modified version, this will allow you to trigger the functions without pressing the Fn key.

Note: By using this modified VoodooPS2, the original "stop" function assigned to F10 will be replaced by "F13", you can go to System Preferences - Keyboard - Shortcuts - Launchpad & Dock, enable Show Launchpad and change the shortcut from "none" to F13 by pressing F10 without holding Fn key, then you are able to activate Launchpad with F10 key.

Note: Fn key is still required for Backlight control key (F6), Fan control key (G) to trigger.

Note: Fn key is not required for F11 key and F12 key to trigger.

All done, take care and stay at home.

Have a good day.
