---
title: Welcome
tags:
- tag1
- tag2
---
<center>
<font size= "6">Joseph Rivera Datasheet</font><br>
as part of<br>
<font size= "8"> Radiolink </font><br>
for<br>
<font size= "5"> Team 105 </font><br>

**Submission: October, 30, 2026**
</center>

## Introduction

This individual engineering datasheet documents my contributions to RadioLink, a project developed by Team 105 for EGR 304 at Arizona State University. It provides an overview of my subsystem's functionality, hardware components, design decisions, and integration with the overall device.

### Project Summary

RadioLink is a portable, off-grid communication device designed to provide dependable wireless messaging during emergencies or in areas without cellular or internet service. The project emphasizes reliability, portability, and ease of use.

Team 105 consists of four engineering students, each responsible for developing an individual hardware subsystem that contributes to the complete device. My subsystem focuses on user controls and temperature monitoring to support RadioLink's functionality.

For additional information regarding the project's objectives, requirements, and overall design, visit the [Team 105 RadioLink Report](https://asu-egr304-2026-f-105.github.io/EGR304-2026-F-105.github.io/).

### My Contribution

My subsystem incorporates a PIC18F57Q43 Curiosity Nano microcontroller, MCP9700A temperature sensor, and MCP6004 non-inverting operational amplifier for temperature signal processing. Six navigation buttons, a test button, and a red LED provide user interaction and additional functionality.

An LM7805 voltage regulator converts the subsystem's 9 V DC input into a regulated 5 V supply. Communication with other subsystems occurs through UART, with a common ground shared between the team's boards.

Readers can explore the following sections for additional technical information:

**Block Diagram:** Component layout, power distribution, and signal connections.
**Component Selection:** Component comparisons and selection rationale.
**Bill of Materials (BOM):** Required components, quantities, and costs.
**Electrical Schematic:** Detailed electrical connections and circuitry.
**Power Budget:** Current consumption and power requirements.
