---
title: Component Selection
---


**Temperature Sensor**

1. Microchip Technologies MCP9700A-E/TO


    ![](MCP9700A-E-TO.jpg)
    

    * $0.61/each
    * [Link to product](https://www.digikey.com/en/products/detail/microchip-technology/MCP9700A-E-TO/1212508?s=N4IgTCBcDaILIGEAKBOA7ABgwQQLQFEB6AFQHkQBdAXyA)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Cost effective                               | Requires ADC conversion |
    | Easy through-hole soldering                      | Analog signal susceptible to noise                                        |
    | Direct PIC ADC connection |

    

2. Texas Instruments TMP36GT9Z

    ![Temperature Sensor](Screenshot%202026-10-16%20102012.png)

    * $1.85/each
    * [Link to product](https://www.digikey.com/en/products/detail/analog-devices-inc/TMP36GT9Z/820404)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | Wide temperature range                                             | Higher cost      |
    | Simple analog interface                                 | Lower specified accuracy at 25°C |
    | Compatible with 5V supply |

    

3. Texas Instruments TMP235A2DBZR

    ![Temperature Sensor](Screenshot%202026-10-16%20105352.png)
    
    * $0.56/each
    * [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/TMP235A2DBZR/9649793?s=N4IgTCBcDaICoFkAKYDMBWAgmAIgIQC0AlEAXQF8g)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | Cost effective                                             | Difficult for surface-mount soldering      |
    | Small PCB footprint                                 | Different voltage-to-temperature conversion |
    | Good specified accuracy (±1.2°C (±2°C)) |

    


**Choice:** Option 1: MCP9700A-E/TO

**Rationale:** The MCP9700A is not only cost effective, but provides simple and direct integration for the Curiosity Nano that will be used for this part of the product. Although its readings aren't as accurate at the TMP235A2DBZR, readings are still within a ±2°C range, and will have a more reliable method of installation.



**Operational Amplifier**



1. Microchip Technologies MCP6004-I/SL


    ![Op-Amp](mcp6004.jpg)
    

    * $0.53/each
    * [Link to product](https://www.digikey.com/en/products/detail/microchip-technology/MCP6004T-I-SL/523092)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Low power consumption supports an efficient subsystem                               | Lower slew rate than the alternatives. |
    | SOIC-14 package is manageable for PCB assembly                      | Four amplifiers may be unnecessary if only one temperature signal needs conditioning.                                        |
    | Operates directly from the subsystem's 5 V supply |



    

2. Texas Instruments TLV9004IDR

    ![Op-Amp](![Op-Amp](Texas%20Instruments%20TLV9004IDR.png)

    * $0.91/each
    * [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/TLV9004IDR/9674911)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | Lower typical supply current than MCP6004                                             | Four channels may be unnecessary for the current circuit.      |
    | Includes EMI/RFI filtering features                                 | Maximum supply voltage is limited to 5.5 V. |
    | Lower maximum input offset voltage improves potential measurement accuracy |

    



3. Texas Instruments TLV9054IDR

    ![Op-Amp](Texas%20Instruments%20TLV9054IDR.jpg)
    
    * $1.14/each
    * [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/TLV9054IDR/10273198)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | 5 MHz bandwidth provides room for future applications                                             | Higher power consumption than very low-power alternatives      |
    | Low input offset voltage supports accurate sensing                                 | Higher bandwidth is unnecessary for slow temperature measurements |
    | Available in SOIC-14 for PCB integration |



    


**Choice:** Option 1: MCP6004-I/SL

**Rationale:** The MCP6004 was selected as the best operational amplifier for the subsystem for its effective balance between low power consumption, cost-effectiveness, and compatibility with the subsystem's design. Its operating voltage range of 1.8–6 V allows it to function reliably with the team's regulated 5 V power supply. Additionally, its rail-to-rail input and output capabilities make it suitable for amplifying the MCP9700A temperature sensor's analog voltage through a non-inverting amplifier configuration before sending the signal to the PIC18F57Q43 Curiosity Nano's ADC. In comparison, the TLV9054IDR and TLV9004IDR lack the advantages that the MCP6004 holds.
