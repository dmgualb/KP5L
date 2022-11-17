# KP5L
Configuration files for compiling Marlin 2.1.1 for KP5L

Those have worked for me, use at your own risk

Platformio.ini is placed here as an example only. The only line you need to edit is:

default_envs = mks_robin_nano35

*OBS: do NOT use mks_robin_nano35_maple, as there will be a warning during compilation and the final firmware just won't work.

After installing the firmware, it's advisable to run the PID autotune to make the adjustment more toght to your machine.
