# ESP32 Temperature Monitoring System using LM35 and ThingSpeak

## Overview

This project uses an ESP32 microcontroller and an LM35 temperature sensor to measure ambient temperature and upload the data to ThingSpeak for real-time cloud monitoring. The system calculates temperature in both Celsius and Fahrenheit and updates the values every 10 seconds.

## Features

* Real-time temperature monitoring
* LM35 analog temperature sensing
* Temperature display in Celsius (°C)
* Temperature conversion to Fahrenheit (°F)
* Wi-Fi connectivity using ESP32
* Cloud data logging using ThingSpeak
* Continuous monitoring and remote access

## Components Required

* ESP32 Development Board
* LM35 Temperature Sensor
* Breadboard
* Jumper Wires
* Wi-Fi Connection

## Pin Connections

| LM35 Pin | ESP32 Pin |
| -------- | --------- |
| VCC      | 3.3V      |
| OUT      | GPIO 35   |
| GND      | GND       |

## Working Principle

1. The LM35 sensor measures the ambient temperature.
2. The ESP32 reads the analog voltage from the LM35 sensor.
3. The voltage is converted into temperature in Celsius.
4. Celsius is converted to Fahrenheit.
5. Both temperature values are displayed on the Serial Monitor.
6. The ESP32 uploads the data to ThingSpeak every 10 seconds.

## Formula Used

Temperature Conversion:

* Celsius:

  Temperature (°C) = Voltage (mV) / 10

* Fahrenheit:

  Temperature (°F) = (Temperature (°C) × 9/5) + 32

## Serial Monitor Output

```text
Temperature (°C): 23.04
C
temperature: 73.48F
Channel update successful.
```

## ThingSpeak Fields

| Field   | Data             |
| ------- | ---------------- |
| Field 1 | Temperature (°C) |
| Field 2 | Temperature (°F) |

OUTPUT 

https://github.com/PandrangiJahnavi/ESP32_Temperature_Monitoring_System_using_LM35_and_ThingSpeak/blob/main/OUTPUT_vaules.png

https://github.com/PandrangiJahnavi/ESP32_Temperature_Monitoring_System_using_LM35_and_ThingSpeak/blob/main/thinkspeak_graph_output.png


## Applications

* Smart Weather Monitoring
* Industrial Temperature Monitoring
* Greenhouse Automation
* IoT Environmental Monitoring

## Future Improvements

* Add DHT11/DHT22 for humidity monitoring
* OLED/LCD display integration
* Mobile application monitoring
* Temperature alerts via SMS or Email
* Data analytics dashboard

## Technologies Used

* ESP32
* LM35 Temperature Sensor
* Arduino IDE
* Wi-Fi
* ThingSpeak IoT Platform

## Author

**Pandrangi Jahnavi**

Electronics and Communication Engineering (ECE)

IoT | Embedded Systems | Industrial IoT Enthusiast
