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
- // $ ./tools/build_nt_2ndboot_img.py -o flashing_boot.img u-boot.bin *not needed
- //create flashing_boot.img for sdcard
- //create flashing_boot_emmc.img for emmc, need to be padded to 512KB
- $ make mrproper
- //clean up

- Files for emmc bootbata partition
- altboot.img   -> altboot emmc bootdata

- Files for sdcard
- cm7.img       -> cm7 sdcard
- cm9.img       -> cm9 sdcard
- altboot1.img  -> altboot1 sdcard
- altboot2.img  -> altboot2 sdcard
- altboot3.img  -> altboot3 sdcard

- Credits,
-
- bauwks
- fattire 
- mik_os
- Denx
- Ogilvy
- Rebellos
- HD
