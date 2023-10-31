CANBus Info

I am currently running the folowing CANBus configuration on 3 printers.  A Switchwire, a Trident 250 and a Trident 350.

BTT U2C v2.1 

BTT Ebb36 v1.2


CANBus install notes.
After installing the U2C and the EBB36 I originally used the ebb-canbus-v1.2.cfg file and called it out in the printer.cfg.  I stopped doing that and moved everything from ebb-canbus-v1.2.cfg into printer.cfg.  The reson I did that was becasuse I could not save my pid settings as it would error out notbeing able to save it to both files.
As you can see below the Molex Microfit 3.0 connectors are not wired theh same, they are swapped left to right between the U2C v 2.1 and the EBB v 1.2.  This caused me some issues but it was a simple fix to swap wires.
<img width="1264" alt="BTT U2C v2 1 Pinout" src="https://user-images.githubusercontent.com/113078228/199635790-d2f7435b-05f7-4dbd-9f8a-3a08b027d211.png">
![EBB36 V1 2](https://user-images.githubusercontent.com/113078228/199635803-ddfac164-213e-4a69-9fc9-5bd4276daa11.png)

I measured the resistance across the two poins shown below on the EBB36, it needs to read 60 ohms, to get that I needed to put a jumper on the 120r pins on both the EBB36 and the U2C as shown in the pictures below.
![EBB36 Jumper](https://user-images.githubusercontent.com/113078228/199636533-a315baf0-b6bd-46d7-892d-554a1c7ace69.jpg)
<img width="597" alt="U2C V2 1 Jumper" src="https://user-images.githubusercontent.com/113078228/199636545-58b72a53-d772-4f0d-9bb3-ee75bcbf4814.png">

This guide got my U2C v2.1 working.

https://github.com/Esoterical/voron_canbus/tree/main/can_adapter/BigTreeTech%20U2C%20v2.1

https://github.com/Esoterical/voron_canbus/blob/main/toolhead_flashing/README.md


Do not use these.

https://maz0r.github.io/klipper_canbus/controller/u2c.html

https://maz0r.github.io/klipper_canbus/toolhead/ebb36-42_v1.1.html
