---
title: XIAO ESP32-S3
---

### IAO ESP32‑S3
Intro:
The IAO ESP32‑S3 is a modern Meshtastic‑compatible board built on Espressif’s ESP32‑S3 microcontroller. It’s designed for high‑performance mesh communication with improved processing power, dual‑core architecture, and expanded memory compared to earlier ESP32 variants. This makes it a strong candidate for both portable and backbone nodes in Iowa Mesh.

Key Features:
- MCU: Espressif ESP32‑S3 dual‑core processor with Wi‑Fi and Bluetooth 5.0 support
- LoRa Transceiver: Semtech SX1262 for long‑range communication
- Frequency Options: 863–870 MHz or 902–928 MHz
- Memory: Expanded RAM and flash compared to ESP32‑WROOM boards, enabling more complex firmware features
- Interfaces: USB‑C for power and programming, GPIO expansion for sensors or peripherals
- Antenna: SMA or U.FL connector depending on board revision
- Form Factor: Compact PCB designed for easy integration into enclosures

Considerations:
- Newer firmware builds may be required to fully leverage ESP32‑S3 features (ensure Meshtastic version compatibility)
- Power draw is slightly higher than ESP32‑WROOM boards, so battery sizing matters for portable use
- Best suited for backbone or semi‑permanent nodes where processing headroom is valuable
- Less beginner‑friendly than Heltec V3 or T‑Beam due to firmware flashing quirks on ESP32‑S3
- Ideal for advanced operators who want to experiment with expanded features or integrate sensors







{{< imgproc "xiao-esp32s3.jpg" Resize "600x" >}}