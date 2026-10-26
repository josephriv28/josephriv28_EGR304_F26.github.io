---
title: Schematic
---

## Overview

This schematic illustrates the electrical design of an individual subsystem responsible for measuring surrounding temperature, receiving user inputs, and communicating with the other RadioLink subsystems. The MCP9700A-E/TO temperature sensor measures ambient temperature, while an MCP6004 operational amplifier, configured as a non-inverting amplifier, conditions and amplifies the analog signal before it is processed by the PIC18F57Q43 Curiosity Nano microcontroller.

The subsystem includes four directional buttons (UP, DOWN, LEFT, RIGHT) and two action buttons (ENTER, BACK) for user interaction, along with a test button and red LED for debugging and verification. Power is supplied through a 9 V DC adapter and regulated to 5 V using an LM7805 linear voltage regulator, with a 125 mA fuse providing preliminary input protection. Capacitors are incorporated for power stabilization, signal filtering, and button debouncing. UART communication is established through RA3 and RA4 to transmit and receive information between the team's subsystems, which share a common ground while maintaining independent voltage regulation.

![Schematic](Rivera%20Individual%20Subsystem%20Updated.png){style width:"350" height:"300;"}
**Figure 1:** Subsystem schematic for function buttons and temperature sensor.


## Resouces

The schematic as a PDF download is available [*here*](Rivera Individual Subsystem.pdf), and the Zip folder of the project [*here*](Individual Subsystem.zip).
