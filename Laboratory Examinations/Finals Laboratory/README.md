# Finals Laboratory Exam

## Overview
This activity demonstrates a fundamental IoT concept: bridging a physical hardware trigger to a network API. The system uses an Arduino as a physical input device (a button) that communicates with a computer via Serial. A Python script running on the computer acts as a "gateway," translating that serial signal into an HTTP web request that is sent to a remote server.

## Hardware Requirements
* 1 Arduino Uno


* 1 Push Button


* 1 Breadboard


* Laptop/PC with Python and requests library installed


## Code Structure
Arduino Sender (The Trigger)


The Arduino monitors a push button connected to Pin 2. To ensure accuracy, it uses "debouncing" logic, which ignores the tiny electrical noise that happens when a button is pressed. When a clean, stable press is detected, the Arduino sends a specific "Group Number" (e.g., "2") to the computer via the USB Serial connection.

Python IoT Client (The Gateway)


The Python script runs on the computer and continuously listens to the Serial port. When it receives the Group Number from the Arduino, it immediately constructs a web URL (e.g., http://.../led/group/2/toggle) and sends an HTTP GET request to that address. This allows a simple physical button press to trigger complex web-based actions on a remote server.

## Contributors:
John Harold R. Magma <br>
Jemuel Chris N. Ambong <br>
Betina B. Arrojo <br>
Keren G. Dellosa <br>
Jamil S. Mariano <br>
Rachelle Yazmhine C. Mendez <br>
Audric P. Pascual <br>

## Reference
[Prompts used to transact with your selected Generative AI](https://docs.google.com/document/d/1Ph4f8GnvtJRS32F7EDq53SKSUNrVf3dXvfsSIAUVcg0/edit?tab=t.0) <br>
[Transaction ID or the link of the conversation](https://gemini.google.com/share/cd19b5a6c23a)
