# ESP32_wroom_pogo_pin_programmer

This is from tindie: https://www.tindie.com/products/petl/esp32-wroom-pogo-pin-programmer-board/


<img src='https://github.com/petl/ESP32_wroom_pogo_pin_programmer/blob/main/photos/IMG_20220205_232909.jpg' width='100%'>

The USB ESP32 WROOM programmer can flash ESP-WROOM-32 modules in circuit without having to desolder them first. It features 37 pointy pogo pins to be directly pressed onto the ESP. 

You can connect a USB C cable (not included) to it and use Arduino IDE, PlatformIO or others to upload code. It features a RESET circuit similar to nodeMCU so you can upload without having to press a button. IO0 and RESET are still routed to buttons, so the ESP can quickly be reset or put into programming mode manually if needed. 

The USB to serial converter is a CH340, which works natively in the Arduino IDE on Windows, Mac and Linux. The seven most relevant pins (EN, IO0, 5V, 3V3, RX, TX, GND) are broken out and labeled in case you want to use it for something else. Rx and Tx have LEDs on the CH340 for quick feedback. There is a power LED and a LED for IO0. The setting used in the IDE confirmed to be working for me are Board: "ESP32 Dev Module" and Upload Speed: "115200" 

It can also probably flash ESP32-WROOM-32SE, ESP32-WROOM-32E, ESP32-WROOM-32D, ESP32-SOLO-1 and most certainly all others that have the same pinout and spacing. 

The board has all ESP32 pins as pogo pins to be easily connected with the standard 2.54mm (0.1in) headers. Those are not supplied by default, but can easily be added. It has an 3.3V regulator on board which can directly supply the ESP.
