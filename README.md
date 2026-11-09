⚖️ Strain Gauge-Based Load Measurement System

<p align="center">
  **An Arduino-Based Digital Load Measurement System Using HX711**
</p>📌 Project Overview

This project demonstrates a load measurement system using a strain gauge load cell and HX711 amplifier module. The system measures the applied load, processes the sensor readings through a microcontroller, and provides output control based on a predefined threshold.

It combines sensor interfacing, signal processing, and embedded programming to demonstrate a practical application of electronics and instrumentation.

🎯 Project Objectives

- Measure applied load using a strain gauge load cell.
- Interface the load cell with a microcontroller through the HX711 module.
- Obtain and process digital sensor readings.
- Implement threshold-based output control.
- Display measurement readings through the Serial Monitor.

⚙️ Hardware Components

Component| Purpose
Strain Gauge Load Cell| Detects applied load
HX711 Module| Amplifies and converts the sensor signal
Microcontroller| Processes sensor readings
Connecting Wires| Hardware connections
Output Indicators / Connected Devices| Show threshold-based output status

🔌 Pin Connections

Connection| Microcontroller Pin
HX711 DOUT| Digital Pin 4
HX711 SCK| Digital Pin 5
Digital Output 1| Digital Pin 2
Digital Output 2| Digital Pin 3

🔄 Working Principle

1. The load cell detects changes caused by an applied load.
2. The HX711 module amplifies the small electrical signal from the load cell.
3. The microcontroller receives the converted readings.
4. The readings are processed using the HX711_ADC library.
5. The measured value is displayed through the Serial Monitor.
6. A threshold value of 30 is used for output control:
   - When the reading is greater than 30, Digital Pin 2 is set HIGH and Pin 3 LOW.
   - Otherwise, Digital Pin 2 is set LOW and Pin 3 HIGH.

💻 Software and Libraries

- Arduino IDE
- Embedded C/C++ (Arduino programming)
- HX711_ADC Library
- EEPROM Library (conditionally included in the code)

✨ Key Features

- Real-time load measurement.
- Digital signal processing using the HX711 module.
- Serial Monitor output.
- Threshold-based output switching.
- Tare functionality through the Serial Monitor.
- Adjustable calibration factor.

🧪 Calibration

The current code uses a calibration factor of 696.0.

calibrationValue = 696.0;

The calibration factor can be adjusted according to the load cell and calibration procedure to improve measurement accuracy.

📁 Project Files

This repository contains the Arduino source code, project photographs, and demonstration video.

🚀 Future Improvements

- Improve measurement accuracy through calibration.
- Add an LCD or OLED display.
- Introduce adjustable threshold settings.
- Store measurement data for analysis.
- Develop a wireless monitoring interface.

📚 Learning Outcomes

Through this project, I gained practical exposure to:

- Strain gauge-based sensing.
- Load cell interfacing.
- HX711 signal conditioning.
- Microcontroller programming.
- Sensor data acquisition.
- Threshold-based embedded system control.

👩‍💻 Author

Heslia

Electronics and Communication Engineering
CHRIST (Deemed to be University)

---

An academic hands-on project exploring sensor interfacing, measurement systems, and embedded electronics.
