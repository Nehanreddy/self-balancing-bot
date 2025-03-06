#  Self-Balancing Bot

## Overview

The Self-Balancing Bot is a two-wheeled robotic system that maintains its balance using an MPU6050 sensor and an ESP32 microcontroller. It utilizes a PID (Proportional-Integral-Derivative) control algorithm to process real-time sensor data and adjust motor speed accordingly. This project demonstrates the effectiveness of feedback control systems in robotics.

## Features

- **Sensor & Control:**
  - **MPU6050 Sensor:** Measures tilt angle using accelerometer and gyroscope.
  - **PID Control:** Ensures stable balancing by continuously adjusting motor speed.
  - **Complementary Filter:**Reduces sensor noise and improves accuracy.
- **Hardware Components:**
  - **ESP32:** Microcontroller for processing sensor data and controlling motors.
  - **L293D Motor Driver:** Drives two DC motors for movement.
  - **Two DC Motors:** Adjust speed to maintain balance.
  - **Battery Pack:** Two 3.7V batteries for power supply.
  - **Chassis & Wheels** Physical structure of the bot.


## Installation

1. **Clone the repository:**
   
```bash
   git clone https://github.com/Nehanreddy/self-balancing-bot.git
```

2. **Set Up the Development Environment**
    - **Install Arduino IDE and configure it for ESP32.**

    - **Install required libraries:**
       - **MPU6050**
       - **Wire**


3. **Upload the Code**
      - **Open self_balancing_bot.ino in Arduino IDE.**
       - **Select the correct ESP32 board and upload the code.**

4. **Hardware Setup:**
   - **kept images in folder check it** 


## Usage

1. **Power the Bot:**
- **Turn on the power supply to the ESP32 and motor driver.**

2. **System Startup:**
- **The bot initializes the MPU6050 sensor and begins processing tilt angle data.**

3. **Balancing Mechanism**
- **The PID controller continuously adjusts motor speeds to maintain balance.**

4. **Debugging & Monitoring**
- **Use Serial Monitor to observe real-time angle data and PID outputs.**

## Future Improvements

- **Better Filtering - Implement Kalman filter for improved accuracy.**
- **Wireless Control - Add Bluetooth/Wi-Fi remote control.**
- **Obstacle Avoidance - Integrate ultrasonic sensors.**