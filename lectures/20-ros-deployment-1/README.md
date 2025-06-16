# 📖 Overview

**Instructor:** Tarun, Soham  
**Date:** June 11, 2025

---

In this session, we began by introducing the fundamental motivation behind the Robot Operating System (ROS), establishing its importance as a middleware for creating robust and modular robotics software. We emphasized a hands-on approach focused on the integration of software with physical systems.

We then presented a full-fledged demonstration of a ROS 2 system to provide a high-level context, covering the entire pipeline from simulation to hardware. This included a breakdown of core components:

- **TF2 (Transform System):** For managing spatial relationships between different coordinate frames.
- **URDF (Unified Robot Description Format):** To define the robot's physical structure.
- **ros2_control:** As the hardware abstraction layer for interfacing with motors and actuators.
- **Gazebo & RViz:** For high-fidelity simulation and 3D visualization.

This demonstration implicitly covered foundational ROS concepts like nodes, topics, services, and actions. We also discussed how these principles extend beyond ground robots to manipulators and drones.

Finally, we outlined the hands-on portion of the course, emphasizing a modern development workflow using Docker and Devcontainers for creating repeatable and sustainable environments. This leads into the main assignment, where students will implement a teleoperation node, test it in simulation, and deploy it on physical hardware, solidifying the bridge between theory and real-world application.

## 🎓 Capstone Project - Part 1

### 🛠️ Development Environment Setup (Pre-requisite)

Before proceeding with the robot setup, complete the following:

1. Run the installation steps provided here:  
   👉 https://github.com/soham2560/ros2_tutorial_repo

2. Pull the Docker image:
   ```bash
   docker pull ghcr.io/soham2560/humble-garden:latest
    ```
    📦 Image link: [humble-garden container](https://github.com/soham2560/DockerForROS2Development/pkgs/container/humble-garden)

### 🚀 Robot Tele-operation

Choose **one** of the following repositories and follow the instructions to set up your development environment and launch the robot in simulation and real-life:

- [HepoBot GitHub Repository](https://github.com/rtarun1/HepoBot)  
- [MecaBot GitHub Repository](https://github.com/soham2560/MecaBot)

### 🎯 Goal

Successfully launch the robot, and **teleoperate it using an Xbox joystick**.

---

## 🔗 Resources

| Topic/Tool                                 | Link                                                                                                                                      |
|--------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| 📑 Lecture Slides – ROS Deployment Part 1       | [![PDF](https://img.shields.io/badge/Open-Slides-red?logo=adobeacrobatreader&logoColor=white)](./lec-20-ros-deployment-1.pdf)            |
| 📘 Articulated Robotics Tutorials          | [![Visit](https://img.shields.io/badge/Open-Tutorials-brightgreen?logo=readthedocs&logoColor=white)](https://articulatedrobotics.xyz/tutorials/) |
| 📚 Nav2 Documentation                      | [![Docs](https://img.shields.io/badge/Open-Nav2%20Docs-blueviolet?logo=ros&logoColor=white)](https://docs.nav2.org)                      |
| 🏗️ Gazebo Getting Started                  | [![Docs](https://img.shields.io/badge/Open-Gazebo-orange?logo=gazebo&logoColor=white)](https://gazebosim.org/docs/latest/getstarted/)   |


