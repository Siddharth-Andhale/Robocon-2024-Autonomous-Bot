# Robocon 2024 Autonomous Bot

Code and development for the autonomous robot used in the Robocon 2024 competition.

## Table of Contents
- [Introduction](#introduction)
- [Hardware Components](#hardware-components)
- [Software Architecture](#software-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Robocon 2024 autonomous bot is a differential drive robot capable of detecting, picking up, and placing color balls during the competition. It utilizes a Jetson Nano as the main computing board, interfaced with an Arduino Mega for motor control and sensor data acquisition.

## Hardware Components
- Jetson Nano (Small Edge AI Computing board)
- Arduino Mega (motor control and sensor interface)
- Cytron MDD10A motor driver
- Servo motor for claw mechanism
- PCA9685 servo driver
- Encoders for wheel odometry

## Software Architecture
The robot is powered by the ROS2 Foxy framework, running on Ubuntu 20.04 on the Jetson Nano. The key software components include:

- Custom ROS2 packages for robot control, perception, and task management
- YOLO v8 model for color ball detection
- Arduino firmware for motor control and sensor data acquisition
- Communication between Jetson Nano and Arduino Mega via UART

## Installation
1. Clone the repository:
   git clone https://github.com/Siddharth-Andhale/robocon-2024-autonomous-bot.git
2. Install the required dependencies, including ROS2 Foxy and the necessary Python packages.
3. Build the ROS2 packages.
4. Upload the Arduino firmware to the Mega board.

## Usage
1. Launch the ROS2 nodes for the autonomous bot.
2. The robot will follow a predefined path, detect the color balls using the camera and ML model, pick them up with the claw, and place them in the designated silos.
3. Monitor the robot's progress and debug any issues using the ROS2 tools and logging.

## Contributing
We welcome contributions to this project. If you find any issues or have ideas for improvements, please feel free to open an issue or submit a pull request.
