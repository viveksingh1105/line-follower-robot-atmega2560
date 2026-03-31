# Line Follower Robot using ATmega2560 (Embedded Control System)

## Overview

This project implements an autonomous line follower robot using an ATmega2560 microcontroller and IR sensors for path detection. The robot detects a predefined black path on a contrasting surface and adjusts motor motion dynamically to follow the trajectory.

The objective of this project was to gain hands-on experience with embedded control systems, sensor interfacing, and real-time hardware-based motion control logic.

This project was completed in January 2019 as part of my undergraduate Electrical Engineering coursework.

---

## System Architecture

The system consists of the following components:

• IR sensor array for line detection  
• ATmega2560 microcontroller  
• Motor driver module  
• DC motors  
• Chassis platform  
• Battery power supply  

Sensor signals are processed by the microcontroller, which generates control commands for motor actuation through the motor driver interface.

---

## Block Diagram

IR Sensors → ATmega2560 → Motor Driver → DC Motors

(A simplified block diagram is provided to illustrate signal flow in the embedded control loop.)

---

## Working Principle

The robot continuously reads signals from the IR sensors placed at the front of the chassis.

Based on sensor activation:

• center sensor active → robot moves forward  
• left sensor active → robot turns left  
• right sensor active → robot turns right  
• no sensor active → robot searches for line or stops  

This logic enables continuous trajectory correction during motion and allows the robot to follow the predefined path autonomously.

---

## Hardware Components Used

• ATmega2560 microcontroller  
• IR sensors  
• Motor driver module (e.g., L298N)  
• DC motors  
• Robot chassis  
• Battery pack  
• Connecting wires and support electronics  

---

## Control Logic

The control workflow followed a real-time embedded decision loop:

1. Read IR sensor signals
2. Detect relative position of path
3. Generate motor control commands
4. Adjust robot direction
5. Repeat continuously during motion

This sensor-based feedback loop enabled stable path-following behaviour under normal operating conditions.

---

## Implementation

The project involved integration of IR sensor detection with microcontroller-based motor actuation using embedded control logic.

Sensor outputs were interpreted by the controller to determine motion direction, and motor commands were issued through a motor driver interface to achieve trajectory tracking.

---

## Results

The robot successfully followed a predefined black path using sensor-based feedback logic.

The system demonstrated stable tracking behaviour under controlled indoor lighting conditions and validated the effectiveness of real-time sensor-driven motion correction.

---

## My Contribution

This project was completed as part of a team during my undergraduate studies.

My role included:

• integration of IR sensor-based detection logic  
• assisting with hardware setup and system wiring  
• supporting testing and calibration of sensor response  
• validation of motion behaviour during trajectory tracking experiments  

---

## Skills Developed

Through this project, I gained practical exposure to:

• embedded control system workflow  
• microcontroller-based motion control  
• sensor interfacing  
• actuator control integration  
• hardware testing and debugging  
• real-time decision logic implementation  

---

## Future Improvements

Possible extensions to this system include:

• PID-based trajectory tracking for smoother motion  
• speed control optimization  
• obstacle detection integration  
• camera-based path detection  
• wireless monitoring interface  

---

## Note

This project was completed in January 2019 during my B.Tech studies.

Due to the time elapsed since completion, original source code and hardware images are not available. The documentation above reflects the implemented system architecture and control logic used during the project.

---

## Author

Vivek Singh  
M.Sc. Automation and Control  
RPTU Kaiserslautern-Landau
