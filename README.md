# E-Paper-Display-for-Kostal-Solar-Inverter

I developed a small system to show basic information of the Kostal Pico IQ Solar Inverter. I use an ESP32 and a Waveshare 2.7 inch e-paper HAT b/w display. 

You have to add your Wifi information and the local IP address and port of your Kostal Inverter in the respective lines of code.
## Wiring
Busy 27

RST 33

DC 25

CS 26

CLK 18

BIN 23

GND GND

VCC 3.3V

## Setup of local environment

Create a file named "secrets.json" at the root level of your project. Use the values below as a template and fill with your own actual secrets.
```json
{
  "wifi.ssid": "YOUR-WIFI-NAME",
  "wifi.password": "YOUR-WIFI-PASSWORD",
  "inverter.host": "192.168.178.100",
  "inverter.ort": 1502
}
```

## Dependencies
- GxEPD by Jean-Marc Zingg, v 3.1.3 [github repo](https://github.com/ZinggJM/GxEPD).
- ArdiunoJson by Benoit Blanchon, v 6.21.3 [source](https://arduinojson.org/)
