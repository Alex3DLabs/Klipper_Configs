# My Trident 350 build

Meanwell LRS-200-24V

Beacon Probe Rev D https://beacon3d.com/product/beacon/

Octopus V1.1

BTT TMC 2209 Stepper Drivers

Sensorless Homing on X and Y - See info below

EBB36 v1.2 with U2C V2.1

Phaetus Rapido HF

Bondtech LGX-Lite

Titanium Extrusion Backers - No more bed tacos!

Nevermore Micro V5 for 1.8/Trident

Running VEFACH (HEPA + Activcated carbon chamber exhaust mod https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/KevinAkaSam/VEFACH

Ellis Bed fan mod https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/Ellis/Bed_Fans

Chamber Thermistor

Eddy Currents Beacon Probe

Side panel quick release snap latch (these are a lifesaver)

Deck panel Support Clips (no sagging bottom panel)

Great Guide here https://wiki.kb-3d.com/en/home/btt/voron/BTT_EBB36

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
    
  


