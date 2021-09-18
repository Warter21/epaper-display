# HA Sensor ePaper Display
E-Paper display for viewing sensor data from Home Assistant. This firmware is based on **ESPhome**, so you need to install ESPhome and compile .yaml file by yourself.

## Sensors data 
The display shows:
- Time and Date
- Moon
- Internal temperature and humidity
- Openweathermap condition and forecast condition
- Openweathermap pressure
- Openweathermap wind direction and speed
- Openweathermap temperature and humidity

### Hardware:
 1. Waveshare 4.2" ePaper display
 2. ESP8266 Wemos D1 Mini
 3. MaxMacSTN's 3D-Printed Case: [https://www.thingiverse.com/thing:4772803]
 4. Stock M3 Screws from ePaper display 

### Wiring: 
Connecting the display to Wemos D1 Mini is very straightforward.

|ePaper Display Pin| ESP8266 Pin|
|--|--|
| BUSY | GPIO16 |
| RST | GPIO04  |
| DC | GPIO12 |
| CS | GPIO15 |
| CLK | GPIO14 |
| DIN | GPIO13 |
| GND | GND |
| 3.3v | 3.3v |

## How to use?

 1. Install ESPhome on your [computer](https://esphome.io/guides/getting_started_command_line.html) 
 2. Copy yaml file and fonts folder to your ESPhome folder.
 3. Edit your Wi-Fi SSID/Password, sensors entity ID, etc.
 4. Connect hardwares.
 5. Flash the firmware via OTA.
 6. Go to Home Assistant, it should automatically discovered your espHome display. If not, add it manually using IP address via ESPhome integration.
 7. Enjoy!

