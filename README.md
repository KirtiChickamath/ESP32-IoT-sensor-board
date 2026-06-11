# ESP32 IoT Sensor Board

A 4-layer IoT PCB designed in KiCad 9 as part of the **Advanced PCB Design with KiCad 9** course by Dr. Peter Dalmaris.

---

## Overview

This board is a medium-complexity IoT development platform built around the ESP32-C3 microcontroller. It includes power management, wireless connectivity, storage, and environmental sensing. All on a compact 4-layer PCB.

---

## Features

- ESP32-C3-WROOM-02 — WiFi and Bluetooth
- USB-C input with ESD protection (USBLC6) and polyfuse
- LiPo battery management with power-path (MCP73871)
- 3.3V LDO voltage regulator (LM1117)
- USB-to-UART bridge (CP2102N) for programming and debugging
- SPI flash memory (W25Q32)
- MicroSD card slot (SPI mode)
- BME280 — temperature, humidity, and pressure (I2C)
- Ambient light sensor (TEMT6000)
- Microphone with preamplifier (MAX4466)
- Status LEDs — power good, charging, charged
- Boot and EN tactile switches
- GPIO and I2C breakout header
- Test points for SPI signals

---

## Layer Stackup

 Layer - Purpose 

 Top copper - L1 -  Components and signal routing 
 Inner 1 - L2 - Ground plane 
 Inner 2 - L3 - 3.3V power plane 
 Bottom copper - L4 -  Additional signal routing 

---

## Communication Interfaces

 Interface - Connected To 

 SPI - Flash memory, SD card 
 I2C - BME280, OLED header 
 UART - CP2102N (via USB) 
 ADC - Light sensor, microphone 

---

## Schematic

![Schematic](images/schematic.png)

---

## PCB Layout

![Layout](images/layout.png)

---

## 3D View

![3D View](images/3d.png)

---

## Tools Used

- KiCad 
- HQDFM

---

## Course Reference

**Advanced PCB Design with KiCad 9**  
Instructor: Dr. Peter Dalmaris  
Platform: Udemy
