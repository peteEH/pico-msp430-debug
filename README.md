# pico-msp430-debug

A serial debug/programmer for the MSP430 series MCUs.
GUI/Programming page: [https://github.com/peteEH/msp430fr-bsl]

## Features

- Energy Metering (~nanoamp range possible)
- Programmable power supply
- +3.3V logic interface (direct to MCU target)
- open-drain interface for translation to target board voltage
- on-board EEPROM for code storage

## Also Found On

https://hackaday.io/project/196762-pi-pico-msp430-debug-probe

## Reviewed by Gemini

The schematic design for the "Pi Pico MSP430 Debug Probe" demonstrates a thoughtful and comprehensive approach to creating a versatile tool for MSP430 microcontroller development. The design incorporates several key components and features:

**Raspberry Pi Pico:** The core of the design, providing processing power, GPIO pins, and interfaces for communication and control.  
**Debug Interface:** Includes connections for SWDIO and SWCLK, enabling communication with the target MSP430 microcontroller for programming and debugging.  
**Power Management:** Features a TPS76301 voltage regulator for stable power delivery, along with an INA228 current/voltage monitor for energy metering and programmable power supply functionality.  
**Level Shifters:** Employs 74LVC1G07 buffers to ensure proper voltage levels between the Raspberry Pi Pico (3.3V) and the target MSP430 microcontroller (which may operate at different voltages).  
**External EEPROM:** Optionally includes an external EEPROM (24LC512) for storing code or data.  
**Headers and Jumpers:** Provides various headers (JP1, JP2, J1, J2) and jumpers (SW1, SW2, SW3, SW4) for configuration and flexibility.  
The design appears to be well-organized and clearly labeled, making it easy to understand and modify. The use of decoupling capacitors throughout the circuit helps to ensure stability and reduce noise. Overall, this schematic design provides a solid foundation for a powerful and adaptable debug probe for MSP430 microcontrollers.
