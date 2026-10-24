---
title: Individal Block Diagram
tags:
- tag1
- tag2
---

## Overview

This block diagram illustrates the individual subsystem for the user buttons and temperature readings for the Radiolink. This includes how major components of the subsystem are connected, how the power is distributed, and how signals travel between the subsystem and the rest of the team’s device. The subsystem is powered from a shared 5V voltage located on Sultan's board, providing power to the PIC18F57Q43 Curiosity Nano, the MCP9700A temperature sensor, the MCP6004 operational amplifier, and the buttons. The MCP9700A temperature sensor produces an analog voltage signal that passes through the MCP6004, configured as a non-inverting amplifier, to amplify the signal sent to the PIC’s RA0/ADC input for measurement. The non-inverting configuration increases the sensor's output voltage while maintaining its polarity, improving the signal's usable range for ADC measurements. All the user inputs are provided through six buttons connected to digital input pins on the microcontroller. Communication with the rest of the team occurs through Connector 2, which provides RX, TX, 5 V, and GND, allowing both power distribution and bidirectional UART  communication between subsystems.

## Individual Block Diagram 


![Block Diagram Screenshot](Individual%20Block%20Diagram.drawio.png)

