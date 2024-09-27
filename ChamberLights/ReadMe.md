# Chamber LEDs


![ChamberLEDs](https://github.com/user-attachments/assets/cb2f78df-978e-47c7-96dd-e1908cb222dc)



I used this mount https://github.com/VoronDesign/VoronUsers/blob/main/printer_mods/eddie/LED_Bar_Clip/LED_Bar_Clip_Misumi_version2.stl

With these LEDs https://www.amazon.com/dp/B09Z6NBWVL?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1


Leveraging this code in the printer.cfg

```
#####################################################################
#   LED Control
#####################################################################

[output_pin chamberlight]
# Chamber Lighting - HE2 Connector (Optional)
pin: PB11
#pwm:true
shutdown_value: 0
value:1
#cycle_time: 0.01
```
