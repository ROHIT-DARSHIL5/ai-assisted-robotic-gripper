# AI-Assisted Robotic Gripper

### Intelligent Object Detection & Adaptive Motion Control

A robotic manipulation system combining **computer vision, embedded control, tactile sensing, and 3D-printed mechanical design**.

The system uses **YOLO for object detection** and a **3-finger, 6-servo gripper** controlled through Arduino and ESP32 to perform intelligent object manipulation.

---

## Project

<!-- Add your best photo of the completed gripper here -->

<p align="center">
  <img src="docs/images/gripper.jpg" width="700">
</p>

---

## Overview

The goal of this project is to combine **AI-based perception with a physical robotic manipulation system**.

The system integrates:

- YOLO-based object detection
- 3-finger, 6-servo robotic gripper
- Arduino UNO + ESP32
- Force / tactile sensing
- Embedded servo control
- Fusion 360 mechanical design
- 3D-printed components
- Web-based joint control

The project was developed around the challenge of connecting **visual perception, physical sensing, and robotic actuation** into one system.

---

# System Architecture

```text
                ┌──────────────────┐
                │   Camera / Input │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │ YOLO Object      │
                │ Detection        │
                └────────┬─────────┘
                         │
                  Object Position
                  & Dimensions
                         │
                         ▼
                ┌──────────────────┐
                │ Control Logic    │
                └────────┬─────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │ Arduino UNO / ESP32  │
              └──────────┬───────────┘
                         │
                    Servo Control
                         │
                         ▼
              ┌──────────────────────┐
              │ 3-Finger Gripper     │
              │ 6 Servo Actuators    │
              └──────────┬───────────┘
                         │
                         ▼
                  Object Manipulation
                         ▲
                         │
              ┌──────────┴───────────┐
              │ Force / Tactile       │
              │ Feedback              │
              └──────────────────────┘
