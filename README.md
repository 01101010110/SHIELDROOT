# SHIELDROOT

*Hi Friends!*

Today I want to show you how to root your Nvidia Shield, for development purposes, as well as for repairing a bricked system. 

I spent over 80 hours researching how exactly this works, and bricked my system over 30 times to try to figure out every way one could "brick" their system in the process of flash.. and succeeded.. so now you don't have to fail 29 times like I did. :-)

I have created a toolkit that contains all the drivers, files, and some executable adb code I wrote from guides I read. I will credit all my sources as always in a seperate file, saved in the SHIELDROOT folder, as it is very, very many this time. It will also be posted on forums that allow such a massive data dump.

If you prefer, I have attached a standalone ADB executable (powershell) that you can use to manually add the commands. Just right click the batch files, select edit, and you can copy and paste the commands one at time, for troubleshooting purposes.

*DOWNLOAD SHIELDROOT:* 

*Step one:*
Plug your usb hub into the port next to your hdmi.
Plug a usb-c cable into the other port.
You will need an Nvidia Controller, a USB Hub, Portable Drive.
As well as a mouse and controller.

*How to Boot into the bootloader:*
Unplug the power cord from the Shield, then reapply it.
Using your Nvidia Controller, hold A and B until the Bootloader shows.
Select Unlock the bootloader.
Select Factory Data Reset.
Hit Reboot and remove the power cord, then unplug the usb from PC.
Wait a few seconds then add the power cord to the Shield.
Leave  the USBC unplugged from your PC.
Hold A and B to post back into the bootloader.

*Setting up the Shield Drivers:*
Open Device Manager on your PC.
Plug the USBC cable into your PC.
Right click on the new device and hit update driver.
Browse Manually to Shield Drivers.
Then hit, "let me pick from a list".
Select I have a Disk.
Then install the andriod.usb file.

*Rooting the Shield, While Flashing a Custom, Fully Rooted System:*
In SHIELDROOT, Run OEMUnlock.
Unplug the USB-C From the PC and Reapply. (Must do to fix broke fastboot after unlock)
Run ShieldRoot.
This will flash the NVIDIA Developer Rooted images we need to install custom OS and Root.
This will also flash TWRP for us, to recovery as well as boot. 
This purposely bricks the system to run TWRP on boot until we achieve desired results.

*Flashing the OS and optional GAPPS:*
Have Lineage and Gapps saved to a portable drive.
Plug the drive into your usb hub.
Select Install in TWRP and start with Lineage. 
Do the same thing for GAPPS If you want to have your playstore. RECOMMENDED. 
Unless you know what you're doing... and you want Google to not spy on your shield.
The GAPPS Version is the mini TV build so it runs much smoother. 

*Sideloading the Root:*
Go into Advanced on TWRP.
Select Sideload ADB.
Then run the SideloadRootApp.bat file.
Lastly SideloadRootManger.bat file.
Select Reboot system.
Setup your system how you please.

*Unlock Developer Options:*
Go into settings.
Device preferences.
About.
Build, hit build 7 times.
 
*Setting up the ADB Tools for Developers or Pentesters:*
Go into developer options.
Enable USB Debugging, all 4 options including Network debugging.
Take note of your IP address.
Right click AdbConnect.bat and select edit.
Add your IP address there.

Run AdbConnect and select *Allow* on the Shield.
Run AdbConnect again and you will be successfully connected.
You can then get Root Access in ADB by running AdbR00t.bat if you need it.
Otherwise you have full access to push files, read and write over system partitions, etc.

Also included files to reboot the system with one push, AdbReboot.bat
Reboot into the bootloader is included, Bootloader.bat
Take note you are able to drop apps into the SHIELDROOT folder and edit the push apps script.
I will be working on a rom with some of my favorite pen-testing tools, as well as a clean version.
I hope to release it publicly next month.

Thank you to the community for always sharing their knowledge.
Love, Jen

Youtube Vids:
FULL PLAYLIST: https://www.youtube.com/playlist?list=PLErzGEIjyUlyiOLVl4aWDYRW-CJd6yF-N

Website Links:
Listed On Forums and In SHIELDROOT FOLDER
