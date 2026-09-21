# AI-Assisted Robotic Gripper

### Intelligent Object Detection & Adaptive Motion Control

A 3-finger, 6-servo robotic gripper combining **computer vision, tactile sensing, embedded control, and mechanical design** for intelligent object manipulation.

---

## Overview

This project explores the integration of **AI-based object detection with a physical robotic gripper**.

The system combines:

- YOLO-based object detection
- 3-finger, 6-servo robotic gripper
- Arduino UNO and ESP32
- Force / tactile sensing
- Embedded servo control
- Fusion 360 mechanical design
- 3D-printed components
- Web-based joint control

The goal is to enable the gripper to detect an object, estimate its position and dimensions, and perform controlled manipulation.

---

## 🧠 System Architecture

```text
                    Camera / Input
                         │
                         ▼
                ┌─────────────────┐
                │  YOLO Detection │
                └────────┬────────┘
                         │
              Object coordinates
              & dimension estimate
                         │
                         ▼
                ┌─────────────────┐
                │ Control System  │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Arduino / ESP32 │
                └────────┬────────┘
                         │
                    Servo Control
                         │
                         ▼
                ┌─────────────────┐
                │ 3-Finger Gripper│
                └────────┬────────┘
                         │
                         ▼
                  Object Handling

             ┌─────────────────────┐
             │ Force / Tactile     │
             │      Sensing        │
             └──────────┬──────────┘
                        │
                        └──── Feedback
