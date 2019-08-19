# ESP8266_Deauther
Wifi Deauther for ESP8266 chips

This is a simple setup to help you to install https://github.com/spacehuhn/esp8266_deauther "deauther"

Many people have simple issues witht his build due to the drivers and skiping minute details

#########

First any ESP8266 chip will work, although each manufactures set-up may vary slightly

PART 1

    1. First you have to install and open the Arduino IDE.

    2. In Arduino go to File -> Preferences add both URLs in Additional Boards Manager URLs

    http://arduino.esp8266.com/stable/package_esp8266com_index.json
    http://phpsecu.re/esp8266/package_deauther_index.json
    
    3. Go to Tools -> Board -> Boards Manager, search "esp8266" and install esp8266 first, then arduino-esp8266-deauther
    4. Select your board at Tools -> Board and be sure it is at ESP8266 Deauther Modules (and not at ESP8266 Modules)!
          **For me using the ESP8266 Lolin chip I need to select the "NodeMCU (ESP-12 Module"
    5. Download the source code for this project under ESP-86233. You can also clone the project to get the latest changes, but you                   will also get the latest bugs ;).
