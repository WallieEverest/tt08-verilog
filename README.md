# Overview
Bucket Brigade - Analog Delay

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
