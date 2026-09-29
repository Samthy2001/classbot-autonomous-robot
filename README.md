# ClassBot Autonomous Delivery Robot
<img width="1983" height="793" alt="ChatGPT Image Sep 30, 2026, 02_03_54 AM" src="https://github.com/user-attachments/assets/92ce7a45-2afe-4641-afa6-b934517a4188" />

## Overview

ClassBot is a ROS-based autonomous delivery robot developed to automate the transportation of classroom materials such as chalks and dusters between classrooms.

The robot integrates robotics, embedded systems, sensor processing, and autonomous navigation.

The system uses an Arduino Mega 2560 for low-level hardware control and a laptop running ROS Noetic for high-level navigation and decision-making.

---

## Project Objectives

- Develop an autonomous classroom delivery robot.
- Automate classroom material transportation.
- Implement obstacle detection and avoidance.
- Develop route-based autonomous navigation.
- Integrate embedded hardware with ROS communication.
- Enable user interaction during delivery.

---

## System Architecture and Data Flow

ClassBot follows a two-layer control architecture.

High-level processing is performed by ROS Noetic running on a laptop, while the Arduino Mega 2560 manages real-time hardware operations.

System data flow:

    User Command
          |
          ↓
    ROS Noetic Laptop
    (Python Control Logic)
          |
          ↓
    Serial Communication
    (PySerial)
          |
          ↓
    Arduino Mega 2560
          |
    -------------------------
    |                       |
    ↓                       ↓
 Motor Control        Sensor Processing
    |                       |
    ↓                       ↓
 L298N Driver        Ultrasonic Sensors
    |                       |
    ↓                       ↓
 DC Motors          Obstacle Detection
    |
    ↓
 Robot Movement
          |
          ↓
 Classroom Delivery Point
          |
    -------------------------
    |                       |
    ↓                       ↓
 Audio Module        Push Button
 Notification        Confirmation
          |
          ↓
 Continue Next Destination

<img width="1536" height="1024" alt="ChatGPT Image Sep 30, 2026, 02_05_44 AM" src="https://github.com/user-attachments/assets/2bbb64d9-149b-4fe9-99e1-48dde888a526" />

---

## Hardware Components

| Component | Purpose |
|---|---|
| Arduino Mega 2560 | Main embedded controller |
| Laptop | ROS processing system |
| DC Motors | Robot movement |
| L298N Motor Driver | Motor control |
| Ultrasonic Sensors | Obstacle detection |
| Servo Motor | Sensor scanning mechanism |
| ESP8266 Wi-Fi Module | Communication |
| ISD1820 Audio Module | Voice notification |
| Push Button | User confirmation |
| Battery Pack | Power supply |

---

## Software Technologies

- ROS Noetic
- Python 3
- C/C++
- Arduino IDE
- Ubuntu Linux
- PySerial Communication

---

## Working Principle

### Training Mode

- Robot is manually guided through the required route.
- Classroom locations are recorded.
- Route information is stored.

### Autonomous Mode

- Robot starts from the initial position.
- ROS sends navigation commands.
- Arduino controls motors.
- Sensors monitor obstacles.
- Robot reaches classroom locations.
- Audio notification is played.
- User confirms delivery.
- Robot continues to the next location.

---

## Autonomous Features

### Obstacle Detection

Ultrasonic sensors detect obstacles and provide distance information for safe movement.

### Route Navigation

The robot follows predefined classroom routes.

### User Interaction

The push button allows confirmation after delivery.

### Audio Notification

The audio module informs users when the robot arrives.

---

## My Contribution

- Designed and developed the robotic platform.
- Integrated Arduino Mega hardware.
- Implemented motor control.
- Integrated ultrasonic sensing.
- Developed ROS-Arduino communication.
- Worked on obstacle detection.
- Integrated audio notification.
- Tested autonomous delivery functions.

---

## Project Output

The ClassBot prototype demonstrates:

- Autonomous robot movement
- Obstacle detection
- Sensor-based navigation
- Classroom material delivery
- Human interaction system

---

## Challenges

- Sensor calibration.
- Communication between ROS and Arduino.
- Reliable obstacle detection.
- Mechanical stability.
- Power management.

---

## Future Improvements

- Upgrade to ROS 2.
- Implement SLAM navigation.
- Add LiDAR/depth sensors.
- Add AI object recognition.
- Improve multi-stop navigation.
- Develop mobile application control.

---

## Repository Structure

    classbot-autonomous-robot

    ├── README.md
    ├── LICENSE
    │
    ├── images
    │   ├── banner.png
    │   └── system-architecture.png
    │
    ├── Arduino
    │   └── ClassBot_Code.ino
    │
    ├── ROS
    │   ├── nodes
    │   └── packages
    │
    └── Documentation

---

## Technologies Used

- ROS Noetic
- Arduino Mega 2560
- Python
- C/C++
- Embedded Systems
- Robotics
- Automation
- Sensor Integration

---

## Author

**Samthy Shuaib**

Mechatronics Engineering Student

Interested in:

- Robotics
- Embedded Systems
- ROS
- Automation
- Intelligent Systems

GitHub:

https://github.com/Samthy2001
