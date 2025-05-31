# STDCRIUS-FT232RL-Basic-6-pin-Breakout-Board

This project is a schematic design for a CRIUS-style FT232RL USB to Serial breakout board, created using Altium Designer. The board allows for USB communication with microcontrollers and other serial devices using the FT232RL USB-to-UART converter.

## 🔧 Features
- FT232RL USB-to-Serial converter (U1)
- USB Mini-B connector (J2)
- 6-pin serial I/O header (J1)
- TX and RX status LEDs with current limiting resistors
- Power supply decoupling capacitors
- Clean GND connection with polygon pour in PCB layout
  
## 🧩 Schematic Overview
| Component | Description |
|----------|-------------|
| **U1 (FT232RL)** | USB to UART bridge IC from FTDI |
| **J2** | Mini-USB connector for PC interface |
| **J1** | 6-pin header for serial I/O (GND, CTS, VCC, TXD, RXD, DTR) |
| **DS1** | TXLED and RXLED for data activity |
| **R1, R2** | 1kΩ resistors to limit current to LEDs |
| **C2 (0.1µF)** | Decoupling capacitor for 3.3V |
| **C3 (10µF)** | Decoupling capacitor for 5V |
| **GND** | Multiple ground pins connected via polygon pour |

## Pinout (J1 - Serial Header)
| Pin | Signal |
|-----|--------|
| 1   | GND    |
| 2   | CTS    |
| 3   | VCC    |
| 4   | TXD    |
| 5   | RXD    |
| 6   | DTR    |

## Notes
- The FT232RL’s CBUS0 and CBUS1 pins are used for TX and RX LED indicators.
- The board is powered via the USB +5V line.
- Polygon pour on the PCB is used for effective GND distribution.
- VCCIO is connected to +5V, making the UART interface 5V compatible.

## Files Included
- `FT232RL_Schematic.PrjPcb`: Altium project file Description 
- `FT232RL_Schematic.SchDoc`: Main schematic
- (Optional) `FT232RL_PCB.PcbDoc`: PCB layout
- `README.md`: Project documentation


