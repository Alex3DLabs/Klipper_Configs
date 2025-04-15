# Input Shaper for TrIDEX

Switch to T1 before running the shaper_calibrate

For T0 - run: 

```
shaper_calibrate chip=toolboard_0
```
Switch to T1

For T1 - run: 

```
shaper_calibrate chip=toolboard_1
```

Put them in the idex_variables.cfg file. They have to be loaded in manually, it won't work if they are in the printer.cfg

They load in the print_start
