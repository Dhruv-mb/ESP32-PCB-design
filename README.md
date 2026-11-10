ESP32-C3 Mini Evaluation Board

📌 Project Overview

This repository contains the KiCad hardware design files for a custom, compact ESP32-C3 (WROOM-02) mini evaluation board. Designed from scratch, this board functions as a standalone, breadboard-friendly tool tailored for rapid embedded development, IoT prototyping, and testing.

⚙️ Key Hardware Features

Microcontroller Core: Powered by the ESP32-C3-WROOM-02 module, offering Wi-Fi and Bluetooth LE capabilities in a highly compact footprint.

Robust Power Stage: Uses a USB-C receptacle for power input, equipped with ESD protection arrays and pi-filtering to ensure clean power. Voltage is stepped down using an AP2112 3.3V LDO regulator for stable delivery.

Native USB & Programming: The native USB differential pairs (D+ and D-) are routed directly to the microcontroller for seamless firmware flashing and debugging without needing an external UART bridge.

Precise RTC Clocking: Integrates a 32.768 kHz external crystal oscillator with precise load capacitors to support low-power Real-Time Clock (RTC) operations.

Boot & Reset Circuitry: Features hardware-debounced tactile switches with RC filters for manual Reset (EN pin) and Boot mode selection (IO9 strapping pin). Proper pull-up logic is implemented for SPI and Download boot modes.

Expansion & Prototyping: Peripheral GPIOs, 3.3V, and GND are broken out to standard 2.54mm pitch pin headers, perfectly spaced for breadboard integration.

🛠️ Tools Used

EDA Software: Designed using KiCad 9 (Schematic Capture and PCB Layout).

Firmware Target: Can be programmed via Arduino IDE or ESP-IDF using C/C++.

📂 Repository Structure

ESP32.kicad_sch: Schematic file detailing component connections and logical blocks.

ESP32.kicad_pcb: PCB layout file detailing trace routing, component placement, and differential pair routing.

ESP32.kicad_pro: KiCad project file.
