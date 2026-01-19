# Laboratory Activity #3: Fire Sensor Implementation

## Overview

This activity focuses on integrating environmental sensors to create a basic fire detection system. It demonstrates how to read analog data from thermistors and photoresistors, convert those readings into meaningful units (Celsius), and utilize logical conditions to trigger an alarm system.

## Hardware Requirements

* 1 Arduino Uno 



* 1 Thermistor 



* 1 Photoresistor (LDR) 



* 1 Red LED (or Buzzer) 



* Resistors (10kΩ for sensors, 220Ω for LED) 



* 1 Breadboard 




## Code Structure

* **Sensor Data Acquisition (Input)** 




The program utilizes two custom functions to monitor the environment. The `temperatureReading` function captures analog data from the thermistor and converts it into Celsius using a specific mapping formula. Simultaneously, the `brightnessReading` function monitors the photoresistor. Both functions compare their readings against predefined thresholds (50°C and 220 light level) and return a status of `1` (True) if the limits are exceeded.
* **Alarm Logic (Output)** 




The main loop continuously checks the status of both sensors. It uses a logical `AND` operator to ensure that the alarm only triggers if **both** high temperature and high light intensity are detected simultaneously. When this specific condition is met, the system enters an alert state, blinking the notification pin (LED or Buzzer) on and off with a 1-second interval. If either condition drops below the threshold, the alarm remains deactivated.

## Contributors:

Mendez, Rachelle Yazmhine C. 




Arrojo, Betina B. 




Mariano, Jamil S.
