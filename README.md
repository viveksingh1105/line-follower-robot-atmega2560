# Line Follower Robot using ATmega2560

## Overview

This project implements an autonomous line follower robot using the ATmega2560 microcontroller and IR sensors. The robot detects a predefined path (black line on a white surface) and adjusts its movement dynamically to follow the trajectory.

The objective of this project was to gain hands-on experience with embedded systems, sensor interfacing, and real-time control logic implementation.

---

## System Architecture

The system consists of:

- ATmega2560 microcontroller
- IR sensor array for line detection
- Motor driver module
- DC motors
- Power supply unit

The IR sensors detect the line position and send signals to the microcontroller, which processes the data and controls motor direction accordingly.

---

## Working Principle

The robot continuously reads input from the IR sensors.

Based on sensor output:

- If the center sensor detects the line → robot moves forward
- If the left sensor detects the line → robot turns left
- If the right sensor detects the line → robot turns right
- If no sensor detects the line → robot stops or searches for the line

This logic enables the robot to follow the path autonomously.

---

## Hardware Components Used

- ATmega2560 microcontroller
- IR sensors
- Motor driver module (e.g., L298N)
- DC motors
- Chassis
- Battery pack
- Connecting wires

---

## Control Logic

The microcontroller continuously monitors sensor signals and executes conditional control logic:

1. Read IR sensor values
2. Determine line position
3. Adjust motor direction
4. Repeat loop in real-time

This closed-loop behaviour enables smooth navigation along the path.

---

## Implementation

The control algorithm was implemented in embedded C and deployed on the ATmega2560 platform.

Sensor readings were processed in real time to generate appropriate motor control signals through the motor driver module.

---

## Results

The robot successfully followed a predefined black path with stable tracking performance under normal lighting conditions.

The project demonstrated reliable sensor-based navigation and real-time embedded control execution.

---

## Skills Developed

Through this project, I gained experience in:

- Embedded systems programming
- Sensor interfacing
- Microcontroller-based control
- Motor driver integration
- Real-time decision logic implementation
- Hardware debugging and testing

---

## Future Improvements

Possible future enhancements include:

- PID-based control for smoother motion
- Speed optimization
- Obstacle detection integration
- Wireless monitoring capability
- Camera-based path detection

---

## Author

Vivek Singh  
M.Sc. Automation and Control  
RPTU Kaiserslautern-Landau
