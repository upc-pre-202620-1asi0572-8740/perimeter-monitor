# Perimeter Monitor

A smart perimeter monitoring system built with ESP32, utilizing 4 Passive Infrared (PIR) sensors to detect motion in four directions (North, East, South, West). The system provides visual feedback via LEDs and displays real-time status on an I2C LCD.

## Features

- **Directional Motion Detection**: Independent PIR sensors for North, East, South, and West.
- **Visual Indicators**: Dedicated LEDs for each direction that toggle upon motion detection.
- **LCD Status Display**: 16x2 I2C LCD showing the current status of all zones.
- **Asynchronous Operation**: Built using the `ModestIoT` library for efficient event handling.

## Hardware Components

- ESP32 Development Board
- 4x Passive Infrared (PIR) Sensors
- 4x LEDs
- 16x2 I2C LCD Display
- Connecting wires and resistors

## Pin Mapping

| Component | Direction | ESP32 Pin |
|-----------|-----------|-----------|
| PIR Sensor| North     | GPIO 4    |
| PIR Sensor| East      | GPIO 18   |
| PIR Sensor| South     | GPIO 26   |
| PIR Sensor| West      | GPIO 32   |
| LED       | North     | GPIO 5    |
| LED       | East      | GPIO 19   |
| LED       | South     | GPIO 27   |
| LED       | West      | GPIO 33   |
| LCD (SDA) | -         | GPIO 21 (Default)|
| LCD (SCL) | -         | GPIO 22 (Default)|

## Software Requirements

The following libraries are required (as specified in `libraries.txt`):
- `ModestIoT` (Wokwi version)
- `LiquidCrystal I2C`
- `ArduinoJson`
- `PubSubClient`
- `ESP32Servo`
- `DHT sensor library`
- `Adafruit Unified Sensor`
- `EspSoftwareSerial`
- `HX711 Arduino Library`

## Installation and Usage

1.  Clone this repository.
2.  Open `sketch.ino` in the Arduino IDE or your preferred environment.
3.  Ensure you have the ESP32 board package installed.
4.  Install the required libraries listed above.
5.  Connect the hardware according to the [Pin Mapping](#pin-mapping).
6.  Upload the code to your ESP32.

### Simulation

This project is configured for simulation on [Wokwi](https://wokwi.com). You can use `wokwi-project.txt` and `diagram.json` to run the project in a simulated environment.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

Developed by the **IoT Solution Development Team**.