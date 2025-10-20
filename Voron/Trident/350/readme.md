# My Trident 350 build

Meanwell LRS-200-24V

Beacon Probe Rev D https://beacon3d.com/product/beacon/

Octopus V1.1 flashed with CANBus firmware

BTT TMC 2209 Stepper Drivers

Sensorless Homing on X and Y - See info below

EBB36 v1.2

Phaetus Rapido HF

[AE Xol Toolhead](https://github.com/Armchair-Heavy-Industries/Xol-Toolhead)

[WWG2 Extruder](https://github.com/tetsu97/WristWatch-G2-Extruder)

Titanium Extrusion Backers - No more bed tacos!

# Colors used

Formbot Black Frame

Atomic Black ABS

Atomic Dark Cherry Red ABS

Atomic Light Grey ABS

# Mods

[Clee's BFI](https://github.com/clee/VoronBFI)

Nevermore Micro V5 for 1.8/Trident

[v2.4 Aire Filter](https://github.com/VoronManiac/V2.4-Aire/blob/main/README.md)

Chamber Thermistor

Side panel quick release snap latch (these are a lifesaver)

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
    
  


