**# Laboratory Activity #2: Working With Analog Signals

## Overview

This activity demonstrates how to implement a sequential light pattern using `analogWrite()` and `while()` loops. It highlights the use of arrays for efficient pin management and analog signal generation to control LED states.

## Hardware Requirements

* 1 Arduino Uno 



* 5 LEDs (Red, Yellow, Blue, Green, Orange) 



* 5 Resistors 



* 1 Breadboard 




## Code Structure

* **Activation Sequence (Turning ON)** 




The program initializes a counter variable to zero to target the first LED in the array. It enters a `while` loop that continues as long as the counter is less than the total number of LEDs. Inside this loop, the code uses `analogWrite()` to send the maximum value (255) to the current LED, turning it to full brightness. It pauses for one second before incrementing the counter to move to the next LED. This repeats until all LEDs are lit.
* **Deactivation Sequence (Turning OFF)** 




After the activation phase, the counter is reset to zero. The program enters a second `while` loop that iterates through the array in the same order. In this phase, the code sends an analog value of 0 to the current LED, effectively turning it off. After a one-second delay, the counter is incremented to proceed to the next pin. This continues until all LEDs are turned off, after which the main loop restarts.

## Contributors:

Mendez, Rachelle Yazmhine C. 




Arrojo, Betina B. 




Mariano, Jamil S.**
