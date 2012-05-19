- Build instructions:
- 
- Download and install toolchain from:
- "http://www.codesourcery.com/sgpp/lite/arm/portal/release1293". Select the IA32 GNU/- Linux TAR one (MD5: c6930d14801b4fab6705d72df013e58b)

- $ mkdir Android
- $ cd Android
- $ git clone https://github.com/succulent/acclaim_cyanoboot
- $ cd acclaim_cyanoboot
- $ export ARCH=arm
- $ export CROSS_COMPILE=$YOURTOOLCHAINPATH/arm-none-linux-gnueabi-
- $ make omap4430sdp_config
- $ make
- $ ./tools/build_nt_2ndboot_img.py -o flashing_boot.img u-boot.bin
- //create flashing_boot.img for sdcard
- $ make mrproper
- //clean up

- boot.img      -> cm7 sdcard boot.img
- altboot.img   -> cm9 sdcard boot.img
- altboot1.img  -> Alternate 1 sdcard boot.img
- altboot2.img  -> Alternate 2 sdcard boot.img
- altboot3.img  -> Alternate 3 sdcard boot.img

- Credits,
-
- bauwks
- fattire 
- mik_os
- Denx
