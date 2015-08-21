

**[ROM][5.1.1] The Android Open Source Project**

[AOSP](http://forum.xda-developers.com/moto-g-2014/development/rom-android-source-project-t3123109/) project from XDA

***How can I install it?***

***Requires Unlocked Bootloader & a custom recovery***

1. Place ROM & Gapps in your SD
2. Reboot in Bootloader Mode
3. Go to "Recovery" (Vol -) and confirm (Vol +)
4. Wipe Data/Factory Reset
5. Wipe Dalvik cache
6. Install the ROM zip
7. Install the Gapps zip
8. Reboot

Upgrading Bootloader

**To Access Bootloader**

    Go to "Recovery" (Vol -) and confirm (Vol +)

Open terminal in the BL folder (or cd to it), plug device to PC.

***Shift +Right click on the folder***

    adb reboot bootloader

Check your current bootloader :

    fastboot getvar version-bootloader
    
Then flash the new one:

    fastboot flash motoboot motoboot.img
    
Reboot the bootloader:

    fastboot reboot-bootloader
    
Re-check its version:

    fastboot getvar version-bootloader
    
**Download Motorola Device Driver**

From the [site](https://motorola-global-portal.custhelp.com/app/answers/prod_detail/a_id/97326/p/30,6720,9050)
    
