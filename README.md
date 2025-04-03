# PID-FOR-MAZE-SOLVER
# 🏁 Maze Solver using PID Control

This repository contains a **PID-controlled maze solver** designed for robotics applications. Using a **Proportional-Integral-Derivative (PID) controller**, the system efficiently navigates a maze, ensuring **smooth movement** and **precise corrections**. By continuously adjusting motor speeds based on sensor feedback, the robot maintains stability and optimizes its path.

## 🚀 Features
✅ **PID-Based Navigation** – Smooth and precise path-following  
✅ **Line & Wall Following Modes** – Supports multiple navigation strategies  
✅ **Real-Time Error Correction** – Dynamically adjusts speed and direction  
✅ **Efficient Path Optimization** – Reduces unnecessary detours  
✅ **Adaptive Control** – Adjusts to varying maze conditions using ToF sensors  

## 🛠️ How It Works
The PID controller computes **error** (deviation from the path) and applies corrections:
- **Proportional (P):** Corrects based on current error.
- **Integral (I):** Eliminates accumulated errors to prevent drift.
- **Derivative (D):** Predicts future errors for smoother adjustments.

ToF sensors ensure precise distance measurements, allowing the robot to maintain a consistent distance from walls and corners for optimized movement.

### **PID Equation**
```math
u(t) = K_p e(t) + K_i \int e(t) dt + K_d \frac{de(t)}{dt}
```

## 📦 Hardware Requirements
- **Microcontroller:** Arduino / Raspberry Pi Pico
- **Time-of-Flight (ToF) Sensors:** VL53L0X, VL53L1X, or similar
- **Motor Driver:** TB6612FNG for efficient motor control
- **Chassis with Motors & Wheels**
- **Power Supply:** Rechargeable Battery Pack or USB Power Source
