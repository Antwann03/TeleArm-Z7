# TeleArm-Z7: FPGA Based Teleporated Robotic Arm Control System
---
This repository will contain project files for TeleArm-Z7, a teleoperated robotic arm developed for the Fall 2026 ECE 520: System on Chip Design course. The goal of the project is to design, build, and program a functional teleoperated robotic arm system. Where it consists of a hand operated master arm and a servo-driven slave arm that's capable of remotely grasping and manipualting objectss

**Performed By:**
- Antonio Anzora Jr

**Professor:**
- Aaron Nanas

# Description 
---
TeleArm-Z7 is a teleoperated robotic arm capable of picking up objects from a distance, with the master and slave arms connected via a 3+ foot UART cable.
# Results and Video Demonstration Links
---

# Background and Methodolgy
---
# Background and Methodology
---
TeleArm-Z7 is a teleoperated robotic arm built around a master-slave architecture. A hand-operated master arm senses joint positions via the Zynq's XADC, while a trigger controls the gripper. This data is sent over UART to a servo-driven slave arm, which mirrors the master's movements to grasp objects from a distance.

The design splits tasks across the Zynq-7000's PS-PL architecture: the PL handles PWM generation and XADC feedback in parallel hardware, while the PS manages control logic and UART communication in software. This lets the system generate servo signals and read sensors simultaneously in real time something a sequential microcontroller like an Arduino or ESP32 can't do without time-slicing.


# Block Diagram
---

# Components Used
---
| Description | Quantity | Manufacturer | Price ($) | Link |
|-------------|----------|--------------|-----------|------|
|Zybo Z7-10 (Zynq-7000 SoC)|1|Digilent|$314.00|[Product Link](https://digilent.com/shop/zybo-z7-zynq-7000-arm-fpga-soc-development-board/)|
|25KG Digital Servo Motor|4|LewanSoul|$13.99|[Product Link](https://www.amazon.com/dp/B0DDKN9RS6?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1)|
|MG995 Server Motor 6 Pack|1|Deego-FPV|$26.99|[Product Link](https://www.amazon.com/dp/B0D7M4LHBP?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1)|

# Pinout Table
---

# CAD & 3D Models
---