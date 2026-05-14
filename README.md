# ESP32-Wi-Fi-LED-Test
Simple ESP32 Wi-Fi test, using arduino IDE 2.3.8 using mobile hotspot
For the use of other ESP boards or other brands changes will be necessary.
Board Used:
ESP32 WROOM-32 Development Board, Wi-Fi, Bluetooth, BLE, 2.4 GHz

Pre Setup:
Install and Open Arduino IDE
File -> Preferences
Find Additional Board Manager URLs
https://espressif.github.io/arduino-esp32/package_esp32_index.json (for my esp)
click Ok
Go Tools -> Board -> Board manager
Search for ESP32
Install ESP32 by the community
After Installation fo Tools -> Boards -> ESP32 (your modle) Boards

Physical Setup:
Mobile:
Make Sure hotspot is on 2.4GHz and 
Hotspot Settings
ssid: espTest
Password: 123456789
Advance Settings:
Security: WPA2-Personal
Hidden Network = Off
Power saving Mode = Off
Wi-Fi sharing = OFF

Pin Congiguration:
3.3 Volt power
Ground 
LED1, 220 Resistor, into GIPO4 (D4)
LED2, 220 Resistor, into GIPO16 (D16)
LED3, 220 Resistor, into GIPO17 (D17)

Libaries Used
WiFi.h
WebServer.h

These Libaries are included within the ESP32 on arduino.

URL is found in the serial Monitor after a successful upload, with full pin and hotspot configuration.
example URL: http://192.168.3.40/
