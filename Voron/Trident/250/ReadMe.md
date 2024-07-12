# My 250x250x250 Trident build information

Meanwell UHP-200-24V

Meanwell UHP-200-48V

Beacon Probe Rev D https://beacon3d.com/product/beacon/

BTT Manta M8P v1.1

BTT TMC 5160 Pro v1.1 Stepper Drivers for X and Y

BTT TMC 2209 Stepper Drivers

Sensorless Homing on X and Y - See info below

BTT EBB36 v1.2

Phaetus Rapido HF

WristWatch Galileo 2

Titanium Extrusion Backers - No more bed tacos!

Nevermore Micro V5 for 1.8/Trident

Ellis Bed fan mod https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/Ellis/Bed_Fans

Chamber Thermistor

BFI

Side panel Annex Panel Clips

Deck panel Support Clips (no sagging bottom panel)

https://www.printables.com/model/595030-side-and-corner-locks/files

Great Guide here https://wiki.kb-3d.com/en/home/btt/voron/BTT_EBB36

https://github.com/kejar31/VoronMods/tree/main/CB-C2

https://github.com/Arksine/CanBoot/issues/61

https://github.com/Esoterical/voron_canbus/tree/main/mainboard_flashing

https://github.com/Klipper3d/klipper/issues/5198

# Sensorless Homing info with Beacon.

I used the Voron Sensorless Homing scripts but I had to add this to the Homing Override section

if home_all or 'Z' in params

    G90
    G1 X175 Y175 F6500
    
    G28 Z
    G1 Z10
