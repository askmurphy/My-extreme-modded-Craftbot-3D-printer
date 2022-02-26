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
* Get some hardware:
* BigTreeTech SKR1.4 (turbo) mainboard
* 4x BigTreeTech TMC2209 stepperdrivers
BigTreeTech TFT3.5 v3.0 display
BigTreeTech BTT Writer v1.0 (optional, WIFI adapter programmer)
35cm neopixel 12volt (60 leds/meter) RGB-ledstrip (we will replace the original white ledstrip)
stepdown XL6009e converter (we need this for the ledstrip)
2x 120cm flatkabel 14wires (display: 3x5 wires, ledstrip: 3 wires)
60cm flatkabel 2wires (for Y-end switch)
2x 240cm wire (for fans)
24v fan (to replace original 12v heaterfan)
2x 24v fan (to replace original 12v objectfans)


# RepRap software setup
* Please follow all the instruction on the firmware-website below.
* To make the Craftbot and SKR1.4 setup more easy for you, here is a full copy of my SDcard which is fitted in the SKR1.4pro mainboard: code/_SDCARD SKR1.4pro.zip

# Marlin software setup (optional)
* For starters, you can use my inital Marlin-setup first, to test your Craftbot with the SKR1.4Pro (without RPI3). You can find the complete Marlin setup code here: code/21-7-2020_CB2_SKR14_Marlin-2.0.x.zip (this will not be updated, totally switched to RepRap now..)

# Used hardware

* [Bigtreetech SKR1.4 pro with 5x TMC2209](https://nl.aliexpress.com/item/4000478858144.html) 

* [Raspberry Pi 3 Model B](https://www.raspberrypi.com/products/raspberry-pi-3-model-b) 

* [RepRapFirmare Raspberry Pi to SKR 1.X Adapter for easy connect (one of Peter’s great creations!)](https://www.tindie.com/products/pcr/reprapfirmware-raspberry-pi-to-skr-1314progtr/) 

* [Bigtreetech TFT3.5 v3.0](https://nl.aliexpress.com/item/4000068088326.html) (optional)

* [Improved heated bed](https://eu.craftbot.com/products/craftbot-plus-pro-glass-build-plate) (optional)

* [Craftbot plus all-metal hotend](https://eu.craftbot.com/collections/spare-parts/products/craftbot-plus-pro-all-metal-hotend
) (optional)

# Used firmware

* [RepRap firmware, created by a few great people!!](https://github.com/gloomyandy/RepRapFirmware) 

# Tips
- get some free time and have patient ;-)


