# Robocon 2024 Autonomous Bot

Code and development for the autonomous robot used in the Robocon 2024 competition.

## Table of Contents
- [Introduction](#introduction)
- [Hardware Components](#hardware-components)
- [Software Architecture](#software-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)

## Introduction
The Autonomous bot we created was a differential drive robot capable of detecting, picking up, and placing color balls during the competition. It utilized a Jetson Nano as the main computing board, interfaced with an Arduino Uno for motor control and sensor data acquisition.

## Hardware Components
- [Jetson Nano](https://developer.nvidia.com/embedded/learn/get-started-jetson-nano-devkit) (Small Edge AI Computing board)
- Arduino Uno (motor control and sensor interface)
- Cytron MDD10A motor driver
- Servo motor for claw mechanism
- PCA9685 servo driver
- Encoders for wheel odometry

## Software Architecture
The robot is powered by the ROS2 Foxy framework, running on Ubuntu 20.04 on the Jetson Nano. The key software components include:

- Custom ROS2 packages for robot control, perception, and task management
- YOLO v8 model for color ball detection
- Arduino firmware for motor control and sensor data acquisition
- Communication between Jetson Nano and Arduino Uno via UART

## Contributing
We welcome contributions to this project. If you find any issues or have ideas for improvements, please feel free to open an issue or submit a pull request.
