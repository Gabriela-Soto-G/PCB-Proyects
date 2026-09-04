# ESP32-Based Motor Power Control System

PCB design for an ESP32-based motor power control system developed in EasyEDA.

## Overview

This project implements a motor power control system using an ESP32 as the main controller.

The design includes an isolated control stage and a power switching stage, allowing the ESP32 to interface with higher-power circuitry while maintaining electrical isolation between the low-voltage control electronics and the power section.

The schematic and PCB were designed in EasyEDA.

## Main Components

- ESP32 DOIT DevKit V1
- H11AA1 optocoupler
- MOC3021-compatible optotriac drivers
- C106D1G thyristor/SCR devices
- Through-hole resistors
- Screw terminal connectors
- Power switching and isolation circuitry

## Project Files

- `1-Schematic_ELPO_ctrl_motor.json` — EasyEDA schematic
- `1-PCB_PCB_ELPO_ctrl_motor.json` — EasyEDA PCB layout

## System Architecture

The design is divided into two main sections:

### Control Stage

The ESP32 provides the control signals required to manage the motor power stage.

Optocouplers are used to electrically isolate the ESP32 from the higher-voltage switching circuitry.

### Power Stage

The power section uses optically isolated drivers and semiconductor switching devices to control the power delivered to the motor.

This architecture helps protect the low-voltage control electronics from the power circuitry.

## How to Open in EasyEDA

1. Open EasyEDA.
2. Go to **File → Open → EasyEDA**.
3. Select the desired `.json` file.
4. Open the schematic or PCB in the editor.
5. Save it into an EasyEDA project if further editing is required.

## Repository Structure

```text
ESP32-Based Motor Power Control System/
├── README.md
├── 1-Schematic_ELPO_ctrl_motor.json
└── 1-PCB_PCB_ELPO_ctrl_motor.json
