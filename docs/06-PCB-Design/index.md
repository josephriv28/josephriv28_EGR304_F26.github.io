
# PCB Design

## Introduction

This page documents the printed circuit board (PCB) design developed for my individual subsystem of the RadioLink project for EGR 304, Team 105. The PCB was designed using KiCad 10 and incorporates the necessary circuitry for temperature monitoring, user input, power regulation, and communication with the other subsystems.

The design includes a PIC18F57Q43 Curiosity Nano microcontroller, MCP9700A temperature sensor, MCP6004 operational amplifier, LM7805 voltage regulator, pushbuttons, and a ribbon cable connector. The PCB layout was developed with consideration for component placement, routing, electrical connectivity, and manufacturing requirements.

## Front PCB Layout

The front side of the PCB contains the component placement and copper routing for the individual subsystem.

![Front PCB Layout](Front_PCB.png)

[Download Front PCB Layout (PDF)](Front_PCB.pdf)

## Back PCB Layout

The back side of the PCB contains the bottom copper layer and additional routing required to complete the electrical connections.

![Back PCB Layout](Back_PCB.png)

[Download Back PCB Layout (PDF)](Back_PCB.pdf)

## KiCad Project Files

The complete KiCad project, including the schematic, PCB layout, and supporting custom libraries, is provided below.

[Download Complete KiCad Project (ZIP)](RadioLink_PCB_Project.zip)

## Gerber Manufacturing Files

The Gerber archive includes the exported manufacturing layers and associated drill files used for design-for-manufacturability verification.

[Download Gerber and Drill Files (ZIP)](Individual_Subsystem_Rivera_Gerber_Files.zip)
