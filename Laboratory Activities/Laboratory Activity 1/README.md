# Laboratory Activity #1: Working With Digital Signals

## Overview
This activity demonstrates how to create a sequential light pattern. The LEDs light up one by one from Pin 12 to Pin 8, and then turn off one by one in the same order

## Hardware Requirements
* 1 Arduino Uno <br>
* 5 LEDs (Red, Yellow, Blue, Green, Orange) <br>
* 5 Resistors <br>
* 1 Breadbord <br>

## Code Structure
* Activation Sequence (Turning ON) <br>
The program begins by setting a counter to target the first LED in the series. It enters a while loop that continues as long as the counter is within the valid range of pins. Inside this loop, the code sends a maximum analog signal (255) to the current LED, turning it on to full brightness. The system then pauses for exactly one second to create a visual step effect before moving the counter to the next LED. This process repeats until all five LEDs are illuminated.

* Deactivation Sequence (Turning OFF) <br>
Once the first phase is complete, the counter resets to the beginning of the array. The program enters a second while loop that iterates through the LEDs in the same order. For this phase, the code sends a minimum analog signal (0) to the current LED, turning it off completely. After waiting for one second, it moves to the next LED. This continues until all lights are extinguished, after which the main loop restarts the entire cycle from the beginning.

## Contributors:
Mendez, Rachelle Yazmhine C. <br>
Arrojo, Betina B. <br>
Mariano, Jamil S.
