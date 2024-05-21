# Sensorless Homing


I have sensorless homing setup on my Voron 0.2 as well as my 350 Trident

Both are running BTT TMC2209 stepper drivers on X & Y

I followed this guide https://docs.vorondesign.com/community/howto/clee/sensorless_xy_homing.html

In both the home macros "_HOME_X" and "_HOME_Y" you will see 
{% set HOME_CURRENT = 0.7 %}
For a better experience change that to 0.5 %

But it wasn't all I needed for my Trident as I am running the Beacon 3d Scanning probe.  See info in my Trident 350 section

On a BTT Octopus v1.1 you have to set the stallguard jumper set per stepper driver to enable sensorless homing and not have any physical endstop switch connected to the endstop port.

<img width="800" alt="Screenshot 2023-11-19 at 2 11 08 PM" src="https://github.com/Alex3DLabs/Klipper_Configs/assets/113078228/9c35a16b-14eb-4889-b0df-4f6825ad7231">

# Make sure that no endstop switches are connected to the ports (in red X).  You will need to install the stallguard jumpers (in yellow) into the stepper driver slots for the homing override.
![PXL_20231120_160407829](https://github.com/Alex3DLabs/Klipper_Configs/assets/113078228/96b2488d-8c57-4b81-86eb-3b6ae1e144e9)
