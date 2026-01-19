# Laboratory Activity #5: Receiving Serial Connection using Arduino from Python

## Overview

This activity demonstrates how to control an Arduino circuit using a Python script running on a computer. Instead of using the built-in Serial Monitor, we use Python to send commands (like 'R' for Red or 'A' for All) through the USB port. The Arduino receives these commands and turns the corresponding LEDs on or off.

## Hardware Requirements

* 1 Arduino Uno 



* 3 LEDs (Red, Green, Blue) 



* 3 Resistors



* 1 Breadboard 



* Laptop/PC with Python installed 




## Code Structure

* **Arduino Firmware (The Receiver)** 




The Arduino code is designed to listen for incoming letters from the computer. It uses a special helper file (`led_control.h`) to organize the functions. When a specific letter is received (like 'R', 'G', or 'B'), the code checks the current state of that LED and flips it (toggles ON or OFF). It also handles commands to turn all lights ON ('A') or OFF ('O').
* **Python Script (The Controller)** 




The Python script creates a simple menu on the computer screen. It connects to the Arduino's specific port. When the user types a choice from the menu, the script sends that letter directly to the Arduino. The script also includes a "clean screen" feature, which wipes the text after every command to keep the interface looking neat and organized.

## Contributors:
Magma, John Harold R. <br>
Ambong, Jemuel Chris N. <br>
Arrojo, Betina B. <br>
Dellosa, Keren G. <br>
Mariano, Jamil S. <br>
Mendez, Rachelle Yazmhine C. <br>
Pascual, Audric P. <br>


### Reference
Model used to generate the content: Gemini 3 Pro
[Prompts used to transact with Generative AI](https://docs.google.com/document/d/1Fe5OqBTM9iATZMIurfX4jmZpX0Domhsl6qaz1dQoqu0/edit?tab=t.0) <br>
[Transaction ID or the link of the conversation](https://gemini.google.com/share/4a584b09de8c)
