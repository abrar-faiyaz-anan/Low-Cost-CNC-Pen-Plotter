# Design and Development of a Low-Cost CNC Pen Plotter Using Recycled Components

This repository contains the documentation, schematic layouts, and control software for a **Low-Cost CNC Pen Plotter** developed as part of the **MTE 3200 Mechatronics Case Study** at the **Department of Mechatronics Engineering, Rajshahi University of Engineering & Technology (RUET)**. The project focuses on sustainable engineering and waste reduction by fabricating a high-precision 2D plotter using repurposed components from discarded electronic devices.

## Project Overview

Commercial CNC machines and automated plotters are often costly and inaccessible for academic prototyping and hobbyists in developing regions. This project demonstrates that precise vector plotting and motion control can be achieved by salvaging stepper motors, slide rails, and mechanical structures from electronic waste (such as old optical disk drives). 

The system relies on an Arduino microcontroller running a modified G-code interpreter firmware to drive dual-axis stepper mechanics alongside a servo-actuated Z-axis pen lifter.

## Key Features

- **Sustainable E-Waste Integration:** Repurposes 4-wire bipolar stepper motors, precision lead screws, and guide rails from discarded DVD/CD drives.
- **Cost-Effective Design:** Achieves high-resolution 2D vector drawing at a minimal manufacturing cost.
- **Microcontroller-Based Control:** Utilizes an Arduino board connected to an L293D motor driver shield to process standard G-code signals.
- **Modular Z-Axis Actuation:** Employs a mini servo motor coupled with a spring-loaded pen holder mechanism for smooth up/down control.

## Hardware Components

1. **Microcontroller:** Arduino Nano / Uno running G-code interpreter firmware.
2. **Actuators:** 2× repurposed micro-stepper motors from optical disk drives (for X and Y axes).
3. **Z-Axis Lift:** 1× micro servo motor for vertical pen engagement.
4. **Driver Circuitry:** L293D Motor Driver Shield.
5. **Power Supply:** 5V 1A DC regulated power adapter.
6. **Chassis & Mechanics:** Recycled slide rails, custom baseplate, and a spring-loaded pen refill mechanism.

## Repository Structure

- `firmware/` - Arduino sketches and modified G-code interpreter source code.
- `hardware/` - Circuit wiring schematics, connection maps, and mechanical assembly layouts.
- `software/` - Utility scripts or instructions for image-to-G-code processing and serial communication senders.
- `docs/` - Project case study report and component datasheets.

## Assembly Instructions

1. **Salvaging Stepper Mechanisms:**
   - Extract optical pickup sliding mechanisms from two scrap DVD/CD drives.
   - Use a multimeter to identify the 4-wire coil pairs (approx. 10 ohms per coil) and solder extension wires.
2. **X-Y Frame Integration:**
   - Mount the X and Y axis rail assemblies at a strict 90-degree angle on a rigid baseplate using secure mechanical fasteners.
3. **Z-Axis Mechanism:**
   - Attach a spring-loaded pen holder onto the X-axis moving carriage.
   - Connect a string from the pen refill to the mini servo motor horn to control vertical translation against the spring tension.

## Installation and Setup

1. **Clone this repository:**
   ```bash
   git clone [https://github.com/username/low-cost-cnc-plotter.git](https://github.com/username/low-cost-cnc-plotter.git)
   cd low-cost-cnc-plotter
