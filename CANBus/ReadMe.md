# Repository for all CANBus related info

# CANBus Info

I am currently running the folowing CANBus configuration on 3 printers.  A Switchwire, a Trident 250 and a Trident 350.

BTT U2C v2.1 

BTT Ebb36 v1.2


# CANBus install notes.
After installing the U2C and the EBB36 I originally used the ebb-canbus-v1.2.cfg file and called it out in the printer.cfg.  I stopped doing that and moved everything from ebb-canbus-v1.2.cfg into printer.cfg.  The reson I did that was becasuse I could not save my pid settings as it would error out notbeing able to save it to both files.
As you can see below the Molex Microfit 3.0 connectors are not wired theh same, they are swapped left to right between the U2C v 2.1 and the EBB v 1.2.  This caused me some issues but it was a simple fix to swap wires.

I measured the resistance across the two poins shown below on the EBB36, it needs to read 60 ohms, to get that I needed to put a jumper on the 120r pins on both the EBB36 and the U2C as shown in the pictures below.

# These guides got me working.

https://github.com/Esoterical/voron_canbus/tree/main/can_adapter/BigTreeTech%20U2C%20v2.1

https://github.com/Esoterical/voron_canbus/blob/main/toolhead_flashing/README.md


Do not use these.

https://maz0r.github.io/klipper_canbus/controller/u2c.html

https://maz0r.github.io/klipper_canbus/toolhead/ebb36-42_v1.1.html

