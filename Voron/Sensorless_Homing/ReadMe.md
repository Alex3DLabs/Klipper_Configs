Sensorless Homing


I have sensorless homing setup on my Voron 0.2 as well as my 350 Trident

Both are running BTT TMC2209 stepper drivers on X & Y

I followed this guide https://docs.vorondesign.com/community/howto/clee/sensorless_xy_homing.html

But it wasn't all I needed for my Trident as I am running the Beacon 3d Scanning probe

On a BTT Octopus v1.1 you have to set the stallguard jumper set per stepper driver to enable sensorless homing and not have any physical endstop switch connected to the endstop port.

<img width="800" alt="Screenshot 2023-11-19 at 2 11 08 PM" src="https://github.com/Alex3DLabs/Klipper_Configs/assets/113078228/9c35a16b-14eb-4889-b0df-4f6825ad7231">


