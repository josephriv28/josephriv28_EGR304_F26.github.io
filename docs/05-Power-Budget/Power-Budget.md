---
title: Power Budget
---

## Overview
The Power Budget was developed to evaluate the electrical requirements of my individual RadioLink subsystem and ensure that the selected power source and voltage regulator can reliably supply its components. This involved calculating the current consumption of the MCP9700A temperature sensor, MCP6004 operational amplifier, and PIC18F57Q43 Curiosity Nano, while accounting for a 25% safety margin. The budget also evaluates the LM7805 voltage regulator and the selected 9V DC power adapter to determine whether sufficient power is available for subsystem operation.


![budget1](Screenshot%202026-10-26%20013847.png){style width:"350" height:"300;"}

![budget2](Screenshot%202026-10-26%20013857.png){style width:"350" height:"300;"}


## Conclusions

From the prepared Power Budget, the subsystem's major components have an estimated total current consumption of 25.692 mA, increasing to 32.115 mA with a 25% safety margin. Including the LM7805's estimated ground current, the total input current is approximately 40.615 mA. The selected AlloverPower 9V, 3A adapter provides sufficient current capacity to support the LM7805 and the subsystem's estimated requirements.

Overall, the Power Budget indicates that the selected power supply and voltage regulator are suitable for the proposed design, with additional capacity available for future development. Final verification of current consumption and regulator performance will be completed through hardware testing.

## Resouces

The power budget as a PDF download is available [*here*](Rivera Power Budget.pdf), and a Microsoft Excel Sheet [*here*](Power Budget Example(1).xlsx).
