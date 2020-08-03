# Ender5PlusMarlin
Configuration files for the Ender 5 Plus with the SKR mini E3 V2 

### Machine Detail:
#### Stock Ender 5 Plus with:
- existing Z Stop
- existing Y Stop
- existing BL Touch


Display changed to TFT35 V3. 0

[Link to Display](https://www.biqu.equipment/products/bigtreetech-tft35-v3-0-display-two-working-modes) 

Board changed to SKR MINI E3 V2. 0

[Link to Board](https://www.biqu.equipment/products/bigtreetech-skr-mini-e3-v2-0-32-bit-control-board-integrated-tmc2209-uart-for-ender-3) 

Extruder and Hotend changed to Swiss Micro Direct Drive Extruder for Ender 5

[Link to Direct Drive Extruder](https://store.micro-swiss.com/collections/extruders/products/micro-swiss-direct-drive-extruder-for-creality-ender-5) 

### Important steps:
- do PID autotune for the hotend `M303 E0 S225 C10` and replace the values at line 495 Configuration.h
- do PID autotune for the heatingbed `M303 E-1 S60 C10` and replace the values at line 541 in Configuration.h 
- after changing values do a `M502 M500` to overwrite the EEPROM with the values provided in the configs.
- calibrate e steps, guide is here: [Extruder Calibration](https://all3dp.com/2/extruder-calibration-6-easy-steps-2/) 

# Current State:
## Problems
- TFT35 has no connection to the printer in Touch mode
## Working
- Autoleveling vith BL TOUCH is working 
- The printer does print
- The prints look OK, some Finetuning has to be done (esteps, belt etc) 
### Overall usable for printing! 

# Work in progress! 
