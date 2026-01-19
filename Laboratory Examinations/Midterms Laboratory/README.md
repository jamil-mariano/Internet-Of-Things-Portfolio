# Midterms Laboratory Examination

## Overview

This activity implements an intelligent lighting control system that monitors environmental brightness using a photoresistor. The system operates in two distinct modes: **Automatic**, which uses pre-set logic to categorize light levels (Cloudy, Normal, Bright), and **Manual**, which allows users to dynamically configure the sensitivity thresholds via Serial commands.

## Hardware Requirements

* 1 Arduino Uno 



* 1 Photoresistor



* 3 LEDs (Green, Yellow, Red) 



* 3 Resistors



* 1 Resistor



* 1 Breadboard 




## Code Structure

* **Command Processing (Input)** 




The system continuously listens for text commands from the Serial Monitor. It parses strings to switch between modes (`MODE AUTO` / `MODE MANUAL`) or to update configuration settings. In **Manual Mode**, users can type `SET LOW <value>` or `SET HIGH <value>` to customize the specific light percentage that triggers the LED changes, allowing for real-time calibration.
* **Adaptive LED Control (Output)** 




Every second, the system reads the light intensity and maps it to a 0-100% scale. It then compares this value against the current thresholds (either the fixed Automatic defaults or the user-defined Manual settings).
* **Green LED:** Activates at low light (Cloudy/Dark).
* **Yellow LED:** Activates at medium light (Normal).
* **Red LED:** Activates at high light (Bright Sunlight).



## Contributors:

Arrojo, Betina B. <br>
Mariano, Jamil S. <br>
Mendez, Rachelle Yazmhine C. <br>
Osit, Eduardo <br>
Pascual, Audric P. <br>

## Reference:
[Prompts used to transact with your selected Generative AI](https://docs.google.com/document/d/157kyq6bmzsTN36vueSw1yjSqWcjcszTZH0mbGn4xpRg/edit?tab=t.0)
[Transaction ID or the link of the conversation](https://gemini.google.com/share/a315dad58546)

