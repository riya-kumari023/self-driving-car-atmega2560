# Smart Autonomous Self-Driving Car

**Description:**  
Autonomous smart car using ATmega2560 and ESP32 with ultrasonic sensors, servo-mounted camera, and robotic arm for obstacle detection, navigation, and object interaction.

---

## Project Overview
This project focuses on building a **self-driving car** capable of navigating autonomously using sensor inputs. The car integrates **ultrasonic sensors** for obstacle detection, a **servo-mounted camera** for visual tracking, and a **robotic arm** for object interaction. The vehicle operates **fully autonomously**, without any manual control.

---

## Key Features
- **Obstacle Detection & Avoidance**: Ultrasonic sensors detect objects and automatically change direction.  
- **Autonomous Navigation**: Car moves without remote control.  
- **Servo-Mounted Camera**: Real-time monitoring of surroundings.  
- **Robotic Arm**: Can pick or interact with objects (prototype).  
- **Modular Architecture**: Easy to upgrade with Raspberry Pi or additional sensors.  

---

## Tech Stack & Hardware
| Component                  | Details |
|----------------------------|---------|
| Microcontroller            | Smartelex ATmega2560, ESP32 |
| Sensors                    | HC-SR04 Ultrasonic Sensor |
| Actuators                  | Servo Motors (Camera + Arm), DC Motors |
| Programming                | Arduino IDE (C++) |
| Communication              | Ethernet (future integration) |

---

## Workflow Diagram
```mermaid
flowchart TD
    A[Ultrasonic Sensor] --> B[ATmega2560 Controller]
    B --> C[Motor Driver → Car Movement]
    B --> D[Servo Motor → Camera/Robotic Arm]
    C --> E[Autonomous Navigation]

**## Results**
  Successfully avoided obstacles in test runs.
  Achieved stable autonomous navigation.
  Robotic arm responds to servo commands for object interaction.
  Prototype demonstrates fully autonomous operation without manual intervention.

**## Future Improvements**
  Full integration with Raspberry Pi 4 for advanced AI-based navigation.
  Object detection with computer vision for the robotic arm.
  Add path-planning algorithms for more complex routes.
