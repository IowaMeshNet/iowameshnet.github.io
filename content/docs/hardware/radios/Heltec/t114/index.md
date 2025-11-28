---
title: Heltec T114
---

### Heltec T114
Intro:
The Heltec T114 is a modular, low‑power Meshtastic‑ready node built on the Nordic nRF52840 platform. It’s designed for flexible power options, outdoor deployments, and expansion with GPS or display modules, making it a versatile choice for both portable and backbone roles.

Key Features:
- Nordic nRF52840 MCU with Bluetooth 5.0 support
- SX1262 LoRa transceiver for long‑range communication
- Frequency options: 433 MHz, 470–510 MHz, 863–870 MHz, 902–928 MHz
- Optional 1.14″ TFT‑LCD display
- Optional GNSS module via dedicated interface
- Multiple power interfaces:
- USB‑C
- 2×1.25 lithium battery connector
- 2×1.25 solar panel connector
- 8×1.25 GNSS interface
- U.FL/IPEX antenna connector for LoRa + integrated 2.4 GHz patch antenna
- Firmware flashing via UF2 drag‑and‑drop (DFU mode with reset button double‑click)

Considerations:
- Optional modules (GPS, display) add cost and complexity — clarify operator needs before purchase
- Requires external antenna for optimal LoRa performance
- Firmware flashing workflow differs from ESP32 boards (UF2 vs USB serial)
- Best suited for solar‑powered or semi‑permanent nodes in outdoor deployments
- More expensive than entry‑level Heltec boards, but offers better modularity and power flexibilit


{{< imgproc "t114.png" Resize "300x" >}}
