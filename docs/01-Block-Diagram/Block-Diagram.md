---
title: Individal Block Diagram
tags:
- tag1
- tag2
---

## Overview

This block diagram illustrates the individual subsystem responsible for user button inputs and temperature readings for the RadioLink. It demonstrates how the major components of the subsystem are connected, how power is distributed, and how signals travel between the subsystem and the rest of the team's device.

The subsystem receives power from an independent 9 V DC power supply, which is regulated to 5 V through an LM7805 linear voltage regulator. This regulated 5 V supply provides power to the PIC18F57Q43 Curiosity Nano, MCP9700A temperature sensor, MCP6004 operational amplifier, and associated user interface circuitry. Unlike the previous design, each team member's subsystem incorporates its own voltage regulator, with only a common ground shared between the subsystems.

The MCP9700A temperature sensor produces an analog voltage signal that passes through the MCP6004, configured as a non-inverting amplifier, before reaching the PIC's RA0/ADC input for measurement. The non-inverting configuration amplifies the sensor's output voltage while maintaining its polarity, improving the signal's usable range for ADC measurements.

User inputs are provided through six buttons connected to the microcontroller's digital input pins. Additional functionality is supported through a test button and LED indicator. Communication with the rest of the team occurs through Connector 2, which provides UART RX and TX connections for serial communication, along with a common GND connection. Each subsystem maintains independent voltage regulation while sharing a common electrical reference for communication.

## Individual Block Diagram 


![Block Diagram Screenshot](Rivera%20Block%20Diagram.drawio.png)

