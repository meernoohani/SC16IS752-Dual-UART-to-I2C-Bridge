# SC16IS752 Dual UART to I2C Bridge

A high-performance bridge board based on the **SC16IS752**, designed to convert an I2C interface into two high-speed UART channels (up to 5 Mbps). This board is ideal for microcontrollers with limited hardware UARTS, such as when adding multiple sensors, GPS modules, or MIDI interfaces to your project. The PCB has been designed in KiCAD V.9.0 and the hardware has also been tested and verified. 


## 🛠 Features
* **Dual UART Channels:** Two independent UARTs (A and B) with 64-byte Send/Receive FIFOs.
* **I2C Interface:** Controlled via a single I2C bus, saving valuable MCU pins.
* **Onboard Crystal:** Integrated 14.7456 MHz crystal for precise baud rate generation.
* **Expanded GPIO:** Provides 8 additional programmable I/O pins (mapped to UART signals or general use).
* **Hardware Flow Control:** Full support for RTS/CTS signaling on both channels.
* **Address Selection:** Onboard jumpers (A0/A1) to easily change the I2C address.
* **Design Tool:** Created with **KiCad 9.0**.

## 📍 Pinout Overview
The board is logically organized for easy wiring:
* **Left Side:** I2C Bus (SCL/SDA), Power (3.3V/GND), and UART Channel A (TX/RX/RTS/CTS).
* **Right Side:** UART Channel B (TX/RX/RTS/CTS) and 8 General Purpose I/Os (GPIO0-GPIO7).
* **Bottom:** Address selection pads (A0, A1) and Interrupt (IRQ) output.
<img width="1723" height="1012" alt="3D_View_front_2" src="https://github.com/user-attachments/assets/b0fcf710-f230-4417-b14a-b0631af18a94" />

## ⚙️ Hardware Specifications
| Parameter | Value |
| :--- | :--- |
| **Supply Voltage** | 3.3V DC |
| **Crystal Frequency** | 14.7456 MHz |
| **Max Baud Rate** | 5 Mbps (at 3.3V) |
| **FIFO Size** | 64 Bytes per channel |
| **I2C Speed** | Up to 400 kHz (Fast-mode) |

## 📦 Production Files
The production-ready files are optimized for **JLCPCB** manufacturing and can be found in the `/JLCPCB Production Files & BOM` folder:
* Gerber and Drill files.
* BOM (Bill of Materials) with LCSC part numbers.
* CPL (Pick-and-Place) files for SMD assembly.

---
*Note: This project is shared for reference and educational purposes.*
