# My extreme modded Craftbot 3D-printer
After some hardware issues I want to upgrade my nice Craftbot Plus 3D-printer, busy for 2 year (allways too little free time), but now ithe mod is almost done and this old printer is alive again makes nice prints!  Time for sharing..

![image](img/modded-craftbot.jpg?raw=true "Modded Craftbot")

| Just a few photo's | will be updated soon! |
|------------|-------------|
| ![Alt text](img/modded-craftbot-BBT-tft35.jpg?raw=true "BTT TFT3.5 v3.0") |
| ![Alt text](img/modded-craftbot-backside.jpg?raw=true "Backside") | 


# Let's MODDING your Craftbot!
* First off all, get the pinout of your new 3D-printer mainboard, I used the SKR1.4 Pro, you can find the pinout image here: img/SKR-V1.4-Turbo-pinout.jpg
* Remove the old Craftbot electronics: mainboard and TFT, we don't need it..
* Get the backplate for the new electronics, you can find it here: https://www.thingiverse.com/thing:4499006
=> I am currently redesign the final version, so wait a moment...
* Nice TFT3.5 case: https://www.thingiverse.com/thing:4839597

* Get some hardware, see list below

# RepRap software setup
* Please follow all the instruction on the firmware-website below.
* To make the Craftbot and SKR1.4 setup more easy for you, here is a full copy of my SDcard which is fitted in the SKR1.4pro mainboard: code/_SDCARD SKR1.4pro.zip

# Marlin software setup (optional)
* For starters, you can use my inital Marlin-setup first, to test your Craftbot with the SKR1.4Pro (without RPI3). You can find the complete Marlin setup code here: code/21-7-2020_CB2_SKR14_Marlin-2.0.x.zip (this will not be updated, totally switched to RepRap now..)

# Used hardware

* [Bigtreetech SKR1.4 pro with 5x TMC2209 stepperdrivers](https://nl.aliexpress.com/item/4000478858144.html) 

* [Raspberry Pi 3 Model B](https://www.raspberrypi.com/products/raspberry-pi-3-model-b) 

* [RepRapFirmare Raspberry Pi to SKR 1.X Adapter for easy connect (one of Peter’s great creations!)](https://www.tindie.com/products/pcr/reprapfirmware-raspberry-pi-to-skr-1314progtr/) 

* [Bigtreetech TFT3.5 v3.0](https://nl.aliexpress.com/item/4000068088326.html) (optional)

* [2x DFRobot Gravity MOSFET Power Controller](https://www.robotshop.com/en/gravity-mosfet-power-controller.html)

* [Improved heated bed](https://eu.craftbot.com/products/craftbot-plus-pro-glass-build-plate) (optional)

* [Craftbot plus all-metal hotend](https://eu.craftbot.com/collections/spare-parts/products/craftbot-plus-pro-all-metal-hotend
) (optional)

* BigTreeTech BTT Writer v1.0 (optional, Marlin only, WIFI adapter * programmer)
* 35cm neopixel 12volt (60 leds/meter) RGB-ledstrip (we will replace the original white ledstrip)

* [stepdown XL6009e converter for ledstrip](https://nl.aliexpress.com/item/32340934616.html)

* flatkabel 10wires (display: 5 wires, ledstrip: 3 wires)
60cm flatkabel 2wires (for Y-end switch)
* 2x 240cm wire (for fans)
* 24v fan (to replace original 12v heaterfan)
* 2x 24v fan (to replace original 12v objectfans)

# Wiring

* Connect the 'RepRapFirmare Raspberry Pi to SKR Adapter' to the RPI3, connect the adapter to SKR:EXP2 using a 10-wire-flatcable and 2x (2x5pins) connectors
* Connect the X-stepper (Craftbot back right stepper) to SKR:XM
* Connect the Y-stepper (Craftbot back left stepper) to SKR:YM
* Connect the Z-stepper (Craftbot back middle stepper) to SKR:ZMA
* Connect the E-stepper (Craftbot extruder stepper) to SKR:E0M
* Connect the X-stop (Craftbot extruder switch) to SKR:X-STOP
* Connect the Y-stop (Inside Craftbot front right switch) to SKR:Y-STOP
* Connect the Z-stop (Inside Craftbot back left switch) to 
SKR:Z-STOP
* Connect the hotend-heater to SKR:E0
* Connect the bed-heater to SKR:HB
* Connect the 24V PSU to SKR:POWER

=> Allways check every connection twice, make sure you use the correct polarity!!


# Used firmware

* [RepRap firmware, created by a few great people!!](https://github.com/gloomyandy/RepRapFirmware) 

# Tips
- get some free time and have patient ;-)


