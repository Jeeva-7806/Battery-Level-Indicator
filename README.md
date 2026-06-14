# Battery-Level-Indicator
Battery Level Indicator
Overview

This project implements a battery level indicator using the LM3914 IC. The circuit visually indicates the charge level of a battery through a series of 10 LEDs. It is suitable for:

Battery monitoring systems
Portable electronic devices
UPS systems
Solar power applications
Rechargeable battery packs
Features
Simple and reliable battery monitoring
10-level LED indication
Dot mode and bar mode operation
Adjustable calibration
Low component count
Easy PCB implementation
Circuit Diagram

Insert Circuit Diagram Here

Components Required
Reference	Value
IC1	LM3914
D1–D10	LEDs
R1	Current limiting resistor
R2	Calibration resistor
R3	Voltage divider resistor
RV1	Potentiometer
SW1	Mode selection switch
Battery	6V/9V/12V (as required)
Working Principle

The battery level indicator circuit is based on the LM3914 LED display driver IC, which converts an analog voltage into a linear LED display.

Voltage Sensing
The battery voltage is applied to the input of the LM3914.
The IC continuously monitors the battery voltage level.
Internal comparators compare the input voltage with preset reference voltages.
LED Indication
Depending on the battery voltage, the corresponding LEDs turn ON.
As the battery voltage increases, more LEDs illuminate.
A fully charged battery lights most or all of the LEDs, while a low battery lights only a few LEDs.
Display Modes
Switch SW1 connected to Pin 9 of the LM3914 selects the display mode:
Dot Mode: Only one LED glows at a time, reducing power consumption.
Bar Mode: All LEDs up to the measured level glow, providing a bar-graph display.
Brightness Control and Calibration
Pins 6 and 7 of the LM3914 are connected through a resistor network that sets the LED current and brightness.
Resistor R3 and potentiometer RV1 form a voltage divider network.
RV1 is used to calibrate the circuit so that the LED indications accurately match the battery voltage range.
Prototype

Insert Prototype Image Here

The prototype demonstrates the practical implementation of the battery level indicator circuit. As the battery voltage changes, the LM3914 drives the appropriate number of LEDs, providing an instant visual indication of the battery charge level.

Applications
Battery chargers
UPS battery monitoring
Solar energy systems
Automotive battery indicators
Portable electronic equipment
Power backup systems
