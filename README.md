# My extreme modded Craftbot 3D-printer
After some hardware issues I want to upgrade my nice Craftbot Plus 3D-printer, this old printer is alive again and makes nice prints!  Time for sharing..

![image](img/modded-craftbot.jpg?raw=true "Modded Craftbot")

My modifications: SKR1.4 Turbo, TFT3.5 v3.0, Reprap firmware, improved hotend, hotend-fan & heated bed, 3 new steppermotors,  2x NEMA17 Vibration Damper Shock Absorbers, filament sensor, RGB ledstrip, etc..
 
| Just a few photo's | Click to enlarge..|
|------------|-------------|
| ![Alt text](img/modded-craftbot-BBT-tft35.jpg?raw=true "BTT TFT3.5 v3.0") | ![Alt text](img/modded-craftbot-wired.jpg?raw=true "Backside") |
| ![Alt text](img/modded-craftbot-rpi-wired.jpg?raw=true "RPi & XL4015 converter") | ![Alt text](img/SKR-V1.4-Turbo-pinout.jpg?raw=true "SKR v1.4 Turbo pinout") |
| ![Alt text](img/usb-panel-mount.jpg?raw=true "Panel mount USB B to USB B cable") | ![Alt text](img/cat6-chassis.avif?raw=true "Devine NCD chassisdeel crystal adapter D-size") |


# Let's MODDING your Craftbot!
* First off all, get the pinout of your new 3D-printer mainboard, I used the SKR1.4 Yurbo
* Remove the old Craftbot electronics: mainboard and TFT, we don't need it..
* Get the backplates for the new electronics, you can find it here: https://www.thingiverse.com/thing:4499006
* Nice TFT3.5 case: https://www.thingiverse.com/thing:4839597

* Get some hardware, see list below

# RepRap software setup
* Please follow all the instruction on the firmware-website below.
* To make the Craftbot and SKR1.4 setup more easy for you, here is a full copy of my SDcard which is fitted in the SKR1.4pro mainboard: code/_SDCARD SKR1.4pro.zip

# Marlin software setup (optional)
* For starters, you can use my inital Marlin-setup first, to test your Craftbot with the SKR1.4Pro (without RPI3). You can find the complete Marlin setup code here: code/21-7-2020_CB2_SKR14_Marlin-2.0.x.zip (this will not be updated, totally switched to RepRap now..)

<strong>WIFI setup</strong>
* https://github.com/luc-github/ESP3D
* https://github.com/luc-github/ESP3D-WEBUI

# <strong>Original Craftbot hardware</strong>
* Meanwell SP-320-24V PSU
* Extruder stepper: 17HS3001-20B
* X,Y, Z steppers: 17HS3001-26B (optional replacement: SL42S247A: 1.8deg.step DC2.5A)


# Used modification hardware

* [Bigtreetech SKR1.4 pro with 4x TMC2209 stepperdrivers](https://nl.aliexpress.com/item/4000478858144.html) 

* [Raspberry Pi 3 Model B](https://www.raspberrypi.com/products/raspberry-pi-3-model-b) 

* [RepRapFirmare Raspberry Pi to SKR 1.X Adapter for easy connect (one of Peter’s great creations!)](https://www.tindie.com/products/pcr/reprapfirmware-raspberry-pi-to-skr-1314progtr/) 

* [Bigtreetech TFT3.5 v3.0](https://nl.aliexpress.com/item/4000068088326.html) (optional)

* [Bigtreetech Filament sensor](https://www.aliexpress.com/item/4000269547406.html) (optional)

* [DFRobot Gravity MOSFET Power Controller](https://www.robotshop.com/en/gravity-mosfet-power-controller.html)

* [Craftbot Improved heated bed](https://eu.craftbot.com/products/craftbot-plus-pro-glass-build-plate) (optional)

* [Craftbot all-metal hotend](https://eu.craftbot.com/collections/spare-parts/products/craftbot-plus-pro-all-metal-hotend
) (optional)

* BigTreeTech BTT Writer v1.0 (optional, Marlin only, WIFI adapter * programmer)
* 35cm neopixel 12volt (60 leds/meter) RGB-ledstrip (we will replace the original white ledstrip)

* [stepdown XL6009e converter for ledstrip](https://nl.aliexpress.com/item/32340934616.html)

* [DC-DC Adjustable Step-down Buck Converter XL4015 5A - with Current Limiter]

* [Panel mount USB B to USB B cable](https://www.kiwi-electronics.nl/nl/panel-mount-usb-b-naar-usb-b-kabel-1629)

* [Devine NCD chassisdeel crystal adapter D-size](https://www.bax-shop.nl/ethernet-chassisdeel/devine-ncd-chassisdeel-crystal-adapter-d-size)

* [2x NEMA17 Vibration Damper Shock Absorber for X and Y-steppers](https://www.aliexpress.com/item/33036894200.html) (optional)

* flatkabel 10wires (display: 5 wires, ledstrip: 3 wires)
60cm flatkabel 2wires (for Y-end switch)
* 2x 240cm wire (for fans)
* 24v fan (to replace original 12v heaterfan)
* 2x 24v fan (to replace original 12v objectfans)
* 1x 12v 60x60x25mm EE60251S1-1000U-999 Sunon fan (optional, to replace old 2410ML-04W-B20 BRUSHLESS FAN 12V Fan inside the original installed PSU)

# Wiring

* Connect the 'RepRapFirmare Raspberry Pi to SKR Adapter' to the RPI3, connect the adapter to SKR:EXP2 using a 10-wire-flatcable and 2x (2x5pins) connectors
* Connect the input of the stepdown XL4015 converter to the 24V PSU, tune the output of the converter to 5Volt
* Connect the 5V/GND of the 'RepRapFirmare Raspberry Pi to SKR Adapter' to the output of the stepdown XL4015 converter
* Connect the X-stepper (Craftbot back right stepper) to SKR:XM
* Connect the Y-stepper (Craftbot back left stepper) to SKR:YM
* Connect the Z-stepper (Craftbot back middle stepper) to SKR:ZMA
* Connect the E-stepper (Craftbot extruder stepper) to SKR:E0M
* Connect the X-stop (Craftbot extruder switch) to SKR:X-STOP
* Connect the Y-stop (Inside Craftbot front right switch) to SKR:Y-STOP
* Connect the Z-stop (Inside Craftbot back left switch) to 
SKR:Z-STOP
* Connect the hotend-heater to SKR:E0
* Connect the hotend-thermistor to SKR:TH0
* Connect the bed-heater to SKR:HB
* Connect the bed-thermister to SKR:TB
* Connect the 24V PSU to SKR:POWER
* Connect DFRobot Gravity MOSFET controller1 VIN/GND to SKR:FAN1
* Connect DFRobot Gravity MOSFET controller1 VOUT/GND to the extruder FAN
* Connect DFRobot Gravity MOSFET controller1 D to SKR:PWRDET
* Connect the Object coolerfan to SKR:FAN0
* Connect the TFT3.5 v3.0 to SKR:TFT using a 5-wire cable.
* Connect the 2 datalines of the LED-strip to SKR:Neopixel
* Connect the input of the stepdown XL6009e converter to the 24V PSU, tune the output of the converter to 12Volt
* Connect the 12V/GND of the LED-strip to the output of the stepdown XL6009e converter

=> ToDo: 
* Case fan (waiting for ordered 24V fan)
* Bigtreetech Filament sensor

=> Allways check every connection twice, make sure you use the correct polarity!!


# Used firmware

* [RepRap firmware, created by a few great people!!](https://github.com/gloomyandy/RepRapFirmware) 

# <strong>PID tuning</strong>
You can find some info about it here: https://3dprintbeginner.com/hotend-and-heatbed-pid-tuning

M303 E0 S245 C8 (extruder)

M303 E-1 S90 C8 (bed)

# Tips
- get some free time and have patient ;-)


