# How it works

ChipTune implements an 8-bit Programmable Sound Generator (PSG).
Input is from a serial UART interface.
Output is PWM audio.

# Overview
This project replicates the Audio Processing Unit (APU) of vintage video games.

# Statistics
- Tiles: 1x2
- DFF: 458
- Total Cells: 2760
- Utilization: 72%

# TinyTapeout 8 Configuration
TT08 devices from the eFabless Multi-Project Wafer (MPW) shuttle are delivered in QFN-64 packages, mounted on a daughterboard for breakout.

Changes:
1.) Static registers addressed by the serial UART have been connected to the external reset, providing a known startup.
2.) Default values for REG signals have been removed, allowing 'X' propagation during simulation until the design reaches steady state.

# How to test

The ChipTune project can be interfaced to a computer COM port (9600,n,8,1).
An analog PWM filter and audio driver are needed for the test rig.

# External Hardware

Computer COM port
