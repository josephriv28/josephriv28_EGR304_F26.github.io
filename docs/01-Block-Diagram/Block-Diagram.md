---
title: Individal Block Diagram
tags:
- tag1
- tag2
---

## Overview

The block diagram provided shows how the major components of the subsystem are connected, how power is distributed, and how signals travel between the subsystem and the rest of the team’s device. The subsystem is powered from the team connection using a 5V LM2596 from Texas Instruments, which provides power to the PIC18F57Q43 Curiosity Nano, temperature sensor, and the buttons. The MCP9700A temperature sensor produces an analog voltage signal that is sent to the PIC’s ADC input for measurement. All the user inputs are provided through six buttons connected to digital input pins on the microcontroller. Communication with the rest of the team occurs through Connector 2, which provides RX, TX, 5 V, and GND, allowing both power and UART data to pass between subsystems.

## Example Block Diagram 

![Block Diagram Screenshot](Screenshot%202026-10-05%20180358.png)
