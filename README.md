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
          **For me using the ESP8266 Lolin chip I need to select the "NodeMCU (ESP-12 Module" Also if your using this chip you need to CHECK THE FAQ for uploading ERRORS!
    5. Download the source code for this project from the releases page. https://github.com/spacehuhn/esp8266_deauther/releases
    6. Extract the whole .zip file, navigate to esp8266_deauther and open esp8266_deauther.ino with Arduino.
    7. Check your upload settings and press upload!
                                                    AFTERWORDS
    
   
        1. Scan for WiFi networks.
        2. Connect to "pwned" with the password "deauther"
        3. Open 192.168.4.1 (or deauth.me)
            **If you don't see a pwned network, flash the ESP8266 again.
            
            HAVE FUN!!!!
    
    FAQ's
    
    These are some small tips that are beneficial for first time users of this software, and hopefully will make it more accessible and cause less headache when flashing the board.
    
    "Flash Button and espcomm_open error"
    
    💥❗️❓❗️❗️💢 Sometimes everything is right but it won't upload and you may get an error like error: espcomm_open failed.
    What you have to do is hold the flash button down, start uploading and only release it when you see that it's started uploading, you can tell if the upload has started as the LED will begin to blink rapidly. At this point you can release the firmware buttton.

    In order to upload successfully, you must select the correct COM port. You can think of it as the address with that your    computer accesses the ESP8266. The best way to find the correct port is to open the Arduino IDE and see what ports are listed there. This looks the same for every OS, including Linux. On Windows, COM1 is usually never the correct port. On Windows you can also have a look at your device manager, there you can also see if a device is not recognized.

    If none of the COM ports work correctly or you can't find any COM Port, you might need to install the drivers.
    The driver you need depends on the UART (USB to Serial) chip that is used on your development board.
    Those are the drivers of the most used chips:

💾 CP2102: https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers
💾 CH340:  https://sparks.gogo.co.nz/ch340.html
