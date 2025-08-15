# My 250x250x250 Trident build information

Meanwell LRS-200-24V

[Beacon Probe Rev D](https://beacon3d.com/product/beacon/)

BTT Octopus V1.1

BTT TMC 2209 Stepper Drivers

Sensorless Homing on X and Y - See info below

BTT EBB36 v1.2

[AE A4T](https://github.com/Armchair-Heavy-Industries/A4T)

Phaetus Rapido Plus HF

[WWG2 Extruder](https://github.com/tetsu97/WristWatch-G2-Extruder)

Titanium Extrusion Backers - Not installed yet.

# Colors Used

LDO Black Frame

Atomic UV Neon Yellow ABS

Atomic Gun Metal Grey ABS

Atomic Light Grey ABS

[Gantry is printed in Ambrosia Galactic Black PC-ABS](https://ambrosiafilament.com/collections/pc/products/ambrosia-pc-abs-filament-of-the-gods-1kg-bambu-ams-friendly-cardboard-spools-premium-3d-printing-filament-house-polycarbonate-abs?variant=47713906557242)

# Mods

Nevermore Micro V5 for 1.8/Trident

Ellis Bed fan mod https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/Ellis/Bed_Fans

Chamber Thermistor

[Clee's BFI](https://github.com/clee/VoronBFI)

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
