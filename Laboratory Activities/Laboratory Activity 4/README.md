# Laboratory Activity #4: Arduino Serial Connection

## Overview

This activity shows how to control the Arduino using the Serial Monitor on your computer. The system turns on a blinking light when a sensor triggers it, and the light stays on until you manually type a command to stop it.

## Hardware Requirements

* 1 Arduino Uno 



* 1 Photoresistor



* 1 LED (Pin 8) 



* 2 Resistors 



* 1 Breadboard 




## Code Structure

* **Checking the Sensor (Trigger)** 




The code constantly reads the light sensor. If the brightness goes above a specific limit (220), it turns on a "blinking mode." Once this mode starts, the LED will keep blinking forever, even if the brightness goes back down to normal.
* **Stopping the Blinking (Reset)** 




To stop the blinking, you must send a command from your computer. The code listens for the word **"stop"** in the Serial Monitor. When it receives this word, it turns off the blinking mode and turns the LED off, resetting the system so it is ready to detect high brightness again.

## Contributors:

Mendez, Rachelle Yazmhine C. 




Arrojo, Betina B. 




Mariano, Jamil S.

### Reference
[Link](https://github.com/jamil-mariano/Internet-Of-Things-Portfolio/blob/main/Laboratory%20Activities/Laboratory%20Activity%204/Act4-References.pdf) 
