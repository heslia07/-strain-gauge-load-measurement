Strain Gauge-Based Load Measurement System

Project Overview

This project demonstrates a load measurement system using a strain gauge-based load cell, an HX711 load cell amplifier and an Arduino-compatible microcontroller.

The system measures the applied load and processes the sensor readings through the HX711 module. Based on the measured value, two digital output indicators respond to a predefined threshold.

Components Used

- Strain gauge-based load cell
- HX711 load cell amplifier module
- Arduino-compatible microcontroller
- Breadboard
- Jumper wires
- LED indicators
- USB cable

Working Principle

1. The load cell senses the applied force or load.
2. The HX711 module amplifies and converts the sensor signal into digital data.
3. The microcontroller reads the data using the HX711_ADC library.
4. The measured value is compared with a threshold of 30.
5. Digital outputs on pins 2 and 3 switch according to the comparison.

Pin Connections

Component| Microcontroller Pin
HX711 DOUT| 4
HX711 SCK| 5
Digital Output 1| 2
Digital Output 2| 3

Software and Libraries

- Arduino IDE
- HX711_ADC library
- EEPROM library (included conditionally in the code)

Calibration

The code uses a calibration factor of 696.0. The system performs tare operation during startup. The tare can also be initiated by sending the character "t" through the Serial Monitor.

Project Demonstration

This repository includes photographs of the hardware setup and a demonstration video showing the project.

Key Learning Outcomes

- Interfacing sensors with a microcontroller
- Understanding strain gauge-based load measurement
- Working with the HX711 amplifier module
- Reading and processing sensor data
- Implementing threshold-based digital output control

Project Files

- "strain_gauge_load_cell.ino" – Arduino source code
- Project photographs – Hardware setup and connections
- Demonstration video – Project operation
