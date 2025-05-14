# EEE3088F_Power_Subsystem_Group61 
The micro-mouse project requires the design and development of a compact, efficient, and reliable power subsystem capable of operating autonomously within a constrained embedded system.
This subsystem will be interfaced with the rest of the micro-mouse through a 2x16-pin header and a JST PH connector for the battery, designed to comply with the physical and electrical constraints specified in the project brief. 

This repository contains the design files and documentation for the power subsystem of an autonomous micro-mouse project developed for EEE3088F 2025. The micro-mouse is designed to navigate and solve mazes autonomously.

# System Architecture
The complete micro-mouse consists of four essential subsystems:

Motherboard - The foundation PCB connecting all other components
Processor Board - Features an STM32L476 microcontroller for computation and control
Sensing Subsystem - Equipped with distance sensors for environmental awareness
Power Subsystem - Focus of this repository

# Power Subsystem Features
The power subsystem is responsible for:

Providing stable 3.3V and 5V power to all micro-mouse components
Controlling up to 4 motors bidirectionally (2 main motors + 2 auxiliary)
Supporting external load switching (2 channels at 1A each)
Real-time power monitoring via INA219 on I2C bus
Battery management for a 1S1P LiPo battery (800mAh 3.7V)
Dual charging modes (200mA and 600mA±100mA)
USB-C power input with 9V Power Delivery negotiation
Power system ON/OFF control with ultra-low standby current (<30μA)
