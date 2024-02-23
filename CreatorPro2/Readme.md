# Unfortunately this project is on hold.  

I was in the process of upgrading my FlashForge Creator Pro 2 so that I can run Klipper on it.  I had it working, I was able to print from each head individually, but never got to the point of calibrating it to print with both heads in an IDEX fashion.  I'll get back to it when I have more time, I have parts that I purchased that will only work on this so I can say it's not going into the junk pile.

# Current mods

BTT Manta M8P v1.1

See my [CreatorPro2/PinOuts.cfg](https://github.com/Alex3DLabs/Klipper_Configs/blob/main/CreatorPro2/PinOuts.cfg) file for into on pins. 

I am updating printer.cfg and will post it soon.

![PXL_20230618_035749435](https://github.com/Alex3DLabs/Klipper_Configs/assets/113078228/5118a282-6573-4337-a04d-e978cfc09022)

![BIGTREETECH MANTA M8P V1 1 PinOut](https://github.com/Alex3DLabs/Klipper_Configs/assets/113078228/c17f7e0f-4f32-42bd-996c-3e52d71a5422)

I ended up soldering two wires to the physical switchs for the Z and Y endstops. 

![RAMPS1 4+Generic M'Bot1](https://github.com/Alex3DLabs/Klipper_Configs/assets/113078228/f590eb77-9d06-4615-b362-a5931916bcfc)

Both X endstops are optical endstops, I ended up making an adapter to put a microswitch endstop in it's place, locatedin the STL directory.

I swapped out the stock extruder stepper motors with 2 Moons extruder stepper motors.

![Moons Steppers](https://github.com/Alex3DLabs/Klipper_Configs/assets/113078228/e8905dbf-b244-461e-84fa-b74b0083ccda)

OEM X Stepper Motors are moons stepping motors type 17hd4063-06n
full_steps_per_rotation: 200
1.8º
