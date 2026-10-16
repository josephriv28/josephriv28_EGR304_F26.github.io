---
title: Component Selection Example
---


**Temperature Sensor**

1. Microchip Technologies MCP9700A-E/TO
    ![](image1.png)

    * $0.61/each
    * [link to product](https://www.digikey.com/en/products/detail/microchip-technology/MCP9700A-E-TO/1212508?s=N4IgTCBcDaILIGEAKBOA7ABgwQQLQFEB6AFQHkQBdAXyA)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Cost effective                               | Requires ADC conversion |
    | Easy through-hole soldering                      | Analog signal susceptible to noise                                        |
    | Direct PIC ADC connection |

2. Texas Instruments TMP36GT9Z

    ![](image3.png)

    * $1.85/each
    * [Link to product](https://www.digikey.com/en/products/detail/analog-devices-inc/TMP36GT9Z/820404)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | Wide temperature range                                             | Higher cost      |
    | Simple analog interface                                 | Lower specified accuracy at 25°C |
    | Compatible with 5V supply |

3. Texas Instruments TMP235A2DBZR

    ![](image3.png)

    * $0.56/each
    * [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/TMP235A2DBZR/9649793?s=N4IgTCBcDaICoFkAKYDMBWAgmAIgIQC0AlEAXQF8g)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | Cost effective                                             | Difficult for surface-mount soldering      |
    | Small PCB footprint                                 | Different voltage-to-temperature conversion |
    | Good specified accuracy (±1.2°C (±2°C)) |


**Choice:** Option 1: MCP9700A-E/TO

**Rationale:** The MCP9700A is not only cost effective, but provides simple and direct integration for the Curiosity Nano that will be used for this part of the product. Although its readings aren't as accurate at the TMP235A2DBZR, readings are still within a ±2°C range, and will have a more reliable method of installation.
