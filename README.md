# KP5L

/MarlinConfigFilesKP5L
Configuration files for compiling Marlin 2.1.1 for KP5L
Platformio.ini is placed here as an example only. The only line you need to edit is:
default_envs = mks_robin_nano35
*OBS: do NOT use mks_robin_nano35_maple, as there will be a warning during compilation and the final firmware just won't work.
After installing the firmware, it's advisable to run the PID autotune to make the adjustment more tight to your machine.

/Marlin2.1.2/WithBLTouch
Configuration files for compiling Marlin 2.1.2 for KP5L
Platformio.ini is placed here as an example only. The only line you need to edit is:
default_envs = mks_robin_nano_v1v2
Enabled:
   BL-TOUCH
   UBL
   Input Shaping
Not enabled:
   Babysteps
   Linear advance
   
 The file tft_fsmc.cpp is patched to avoid SDCARD reading problems with GD32 microcontroller.
 Instead of using this file, it's better to look and apply the patch from here:
 https://github.com/MarlinFirmware/Marlin/commit/1940418bbe89d07863ed05c6cddb1edf285a5a31
   
Those have worked for me, use at your own risk
