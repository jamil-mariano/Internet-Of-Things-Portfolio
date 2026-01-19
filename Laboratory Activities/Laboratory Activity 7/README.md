# Laboratory Activity #7: Web-Controlled LED System using FastAPI

## Overview

This activity bridges the gap between web technologies and hardware control. It implements an HTTP-based solution where an Arduino circuit can be controlled via a web API using Python's **FastAPI** framework. Users can toggle LEDs by simply accessing specific URLs in their browser, effectively turning a computer into a web server for IoT control.

## Hardware Requirements

* 1 Arduino Uno 



* 3 LEDs (Red, Green, Blue) 



* 3 Push Buttons 



* 6 Resistors 



* 1 Breadboard 



* Laptop/PC with Python and `fastapi` installed 




## Code Structure

* **Arduino Sketch (Device Logic)** 




The Arduino acts as the execution unit. It listens for single-character commands sent via the Serial port: `'1'`, `'2'`, and `'3'` toggle the Red, Green, and Blue LEDs respectively, while `'o'` and `'f'` turn all LEDs on or off. Additionally, the sketch monitors physical push buttons; if a button is pressed locally, it toggles the corresponding LED and sends a notification message back to the computer.
* **Python & FastAPI (The Web Server)** 




The Python script functions as a bridge between the user and the hardware. It runs a local web server using FastAPI that defines specific "routes" or URLs (e.g., `/led/red`). When a user visits one of these URLs, the script intercepts the request and sends the corresponding command to the Arduino via the USB serial connection. It also runs a background task to listen for and display any messages coming from the Arduino, such as button presses.

## Contributors:
Magma, John Harold R. <br>
Ambong, Jemuel Chris N. <br>
Arrojo, Betina B. <br>
Dellosa, Keren G. <br>
Mariano, Jamil S. <br>
Mendez, Rachelle Yazmhine C. <br>
Pascual, Audric P. <br>
