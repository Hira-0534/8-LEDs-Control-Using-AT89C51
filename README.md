# 8 LEDs Control Using AT89C51 – Embedded Systems Lab Assignment

This repository contains my Embedded Systems Lab Task developed in the 5th Semester (BS Software Engineering).
The purpose of this assignment was to interface LEDs and push buttons with the AT89C51 microcontroller and simulate the circuit using Proteus 8 Professional.

## Project Overview

This project demonstrates:

- Interfacing 8 LEDs using Port 2
- Interfacing 4 push buttons using Port 3
- Controlling LED pairs based on button input
- Understanding digital input/output behavior
- Testing and verification using Proteus 8 Professional

The system reads button inputs in real-time and turns ON/OFF paired LEDs accordingly.

## Project Screenshots

### 1. Circuit Diagram (Proteus 8 Professional)
images/circuit.png

### 2. Button Press Output
images/output.png

### 3. Simulation Running
images/simulation.png

## Tools & Technologies Used

- AT89C51 Microcontroller
- Proteus 8 Professional (ISIS)
- Embedded System Concepts
- Digital I/O Understanding

## Hardware Components

- AT89C51 Microcontroller
- 8 LEDs (P2.0 – P2.7)
- 4 Push Buttons (P3.0 – P3.3)
- Jumper Wires
- Power (Vcc & GND)

## Working Logic

| Button | Port Pin | LEDs Controlled |
|--------|----------|------------------|
| Button 1 | P3.0 | LED1 and LED3 |
| Button 2 | P3.1 | LED2 and LED4 |
| Button 3 | P3.2 | LED5 and LED7 |
| Button 4 | P3.3 | LED6 and LED8 |

Each button turns ON its assigned pair of LEDs.
Releasing the button turns the LEDs OFF.
## Procedure:
## Step 1: Open Keil µVision
1.	Open Keil µVision on your PC.
2.	Click on Project → New µVision Project.
3.	Choose a folder and name your project .
4.	Select the microcontroller:
o	Go to Atmel → AT89C51 and click OK.
o	When asked to copy startup code, click No.


## Step 2: Write the Code
1.	Click File → New and write code.
2.	Save the file .
## Step 3: Add the File to Project
1.	In the Project window, right-click Source Group 1 → Add Existing Files to Group.
2.	Select your  file and click Add, then Close.
## Step 4: Build the HEX File
1.	Go to Project → Options for Target 'Target 1'.
2.	In the Output tab, check Create HEX File and click OK.
3.	Click the Build/Compile button (or press F7).
4.	Make sure the message says "0 Errors".
5.	A HEX file will be created in your project folder

## Step 5: Open Proteus
1.	Open Proteus software.
2.	Place components:
o	AT89C51 Microcontroller
o	LED
o	Logic state
o	Ground 
3.	Connect LED anode to P2.0 (pin 1) and cathode to GND.
## Step 6: Load HEX File in Proteus
1.	Double-click on the AT89C51 IC in Proteus.
2.	In the Program File section, browse and select the generated .hex file (from Keil project folder).
3.	Click OK.
## Step 7: Run Simulation
1.	Click the Play (Run) button in Proteus.
2.The LED (D1) will turn ON and OFF with the help of logic state.
    Set Logic State = 1 → LED ON,  Set Logic State = 0 → LED OF

## Simulation Summary

- Circuit designed in Proteus 8 Professional
- Buttons act as digital inputs
- LEDs act as digital outputs
- Port 3 reads button states
- Port 2 lights the corresponding LED pairs



## Author

Hira Shahid  
5th Semester — BS Software Engineering  
Mirpur University of Science & Technology (MUST), AJK  
Email: hirashahid756@gmail.com  
GitHub: Hira-0534  

## Academic Note

This project is created for academic and lab assignment purposes only as part of the Embedded Systems Laboratory Course.
