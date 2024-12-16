# M600 Filamanet change at layer


Add a filament change (m600) a the layer in your slicer and it will automatically pause the print when you need to change the filament, it will move the printhead to the front left corner and then unload the filament.  You just need to swap the filament to the next color, and manually extruded until the color runs clear, knock off any excess filament and hit resume.


Download the m600.cfg file, you know you want it.



## How to use the M600 feature

Make sure you have the following in your #Extruder section of your printer.cfg

```
max_extrude_only_distance: 200
max_extrude_cross_section: 50.0
```

Once you have the M600 Macro in your printer config you only need to do a few things.

1 - In SuperSlicer, add the part you want to do a fliament swap on.

2 - Slice it.

3 - Move the slider on the right to the layer you want to change colors, right click on the "+" and choose "Add color change (M600)"

<img width="1573" alt="Screenshot 2024-11-30 at 9 44 31 PM" src="https://github.com/user-attachments/assets/0c06362f-65fa-4ed7-a248-c957deabe1a1">

4 - Pick a color for the swap.

<img width="1447" alt="Screenshot 2024-11-30 at 9 44 42 PM" src="https://github.com/user-attachments/assets/0cc501ff-d5df-4995-be50-77de6310eedd">

5 - close the color box, it will go back to the STL view, then click "slice" again.

6 - you will now see the part in it's gcode sliced view with 2 colors.

<img width="1292" alt="Screenshot 2024-11-30 at 9 44 56 PM" src="https://github.com/user-attachments/assets/2d44a331-6ff1-40a4-aec2-0d6217816f42">


### For OrcaSlicer - I need to test this!

1 - It's similar except you "add custom G-Code"

<img width="1069" alt="Screenshot 2024-11-30 at 10 10 50 PM" src="https://github.com/user-attachments/assets/cec231ba-d9f4-4b42-85ce-770d293e47b6">

2 - Enter "M600" and click ok.

<img width="730" alt="Screenshot 2024-11-30 at 10 11 14 PM" src="https://github.com/user-attachments/assets/3b1d568a-91e2-4787-9550-26733550153d">

3 - Slicer the part again.
