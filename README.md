# IR Sensor Array PCB

A custom IR sensor array PCB designed in EasyEDA for line-following and autonomous mobile robot applications. This project aims to provide a wide-field sensor arrangement capable of accurate line detection, intersection recognition, and robust path tracking for high-speed robotics competitions.

## Project Overview

Traditional line-following robots often use a straight-line arrangement of infrared sensors. This project explores a curved sensor layout that increases lateral coverage and allows the robot to detect turns and deviations earlier.

The board uses multiple TCRT5000 reflective infrared sensors arranged in an arc around the front of the robot. Sensor outputs are routed through a DB9 connector for easy integration with microcontrollers such as Arduino, ESP32, STM32, or Raspberry Pi Pico.

## Features

* Custom PCB designed using EasyEDA
* Multiple TCRT5000 reflective IR sensors
* Wide-angle sensor coverage
* Compact robotics-oriented form factor
* DB9 interface connector
* Suitable for PID-based line following
* Designed for competition robots
* Expandable architecture for larger sensor arrays

## Hardware Design

### Sensor Configuration

The array consists of multiple TCRT5000 infrared reflective sensors positioned in a curved layout.

Advantages of the curved arrangement include:

* Earlier turn detection
* Improved corner handling
* Better line recovery
* Wider sensing region
* Enhanced intersection detection

### Working Principle

Each TCRT5000 sensor emits infrared light toward the surface below.

* White surfaces reflect infrared light.
* Dark lines absorb infrared light.
* The reflected intensity changes the phototransistor output.
* A microcontroller reads the sensor states and determines line position.

The resulting data can be used by control algorithms such as PID to steer the robot accurately along a path.

## Repository Structure

```text
IR-Sensor-Array/
├── PCB/
│   ├── Schematic
│   ├── PCB Layout
│   └── Gerber Files
│
├── Images/
│   ├── PCB_Render.png
│   ├── PCB_Layout.png
│   └── Schematic.png
│
├── Documentation/
│   └── Design Notes
│
└── README.md
```

## Design Software

* EasyEDA
* KiCad (future compatibility planned)

## Applications

* Line follower robots
* Autonomous navigation systems
* Robotics competitions
* Educational robotics platforms
* Research and prototyping projects

## Future Improvements

* 16-sensor version
* Adjustable sensitivity control
* Integrated comparator stage
* Analog output support
* On-board status indicators
* Modular connector system

## Project Status

🚧 Work In Progress

The PCB design is currently under development and validation. Future revisions will focus on sensor optimization, signal reliability, and real-world testing on autonomous robots.

## Author

Shreyas Pai

Electronics, Robotics, and Embedded Systems Enthusiast
