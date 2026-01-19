# Laboratory Activity #6: Bidirectional Control Using Arduino and Python

## Overview

This activity demonstrates how to create a two-way communication system between an Arduino and a Python script. The project establishes a control loop where the Arduino sends inputs (button presses) to the computer, and the Python script responds by sending commands back to control the LEDs.

## Hardware Requirements

* 1 Arduino Uno 



* 3 LEDs (Red, Green, Blue) 



* 3 Push Buttons 



* 6 Resistors 



* 1 Breadboard 



* Laptop/PC with Python installed 




## Code Structure

* **Arduino Code (Hardware Manager)** 




The Arduino performs two main tasks simultaneously. First, it monitors the three buttons using a "debounce" technique to ensure that a single press is registered cleanly without signal noise. When a button is pressed, it sends a specific letter ('R', 'G', or 'B') to the computer. Second, it listens for incoming numbers ('1', '2', '3') from the Python script to toggle the corresponding LEDs on or off.
* **Python Script (Logic Controller)** 




The Python script acts as the decision-maker in the system. It connects to the Arduino and continuously checks for incoming data. When it receives a signal indicating a button press, the script processes the input and immediately sends a command back to the Arduino to update the LED status. This setup allows the computer to manage the logic while the Arduino handles the physical components.

## Contributors:
Magma, John Harold R. <br>
Ambong, Jemuel Chris N. <br>
Arrojo, Betina B. <br>
Dellosa, Keren G. <br>
Mariano, Jamil S. <br>
Mendez, Rachelle Yazmhine C. <br>
Pascual, Audric P. <br>
