# 📖 Overview
**Instructor:** Soham, Tarun  
**Date:** June 12, 2025

---

In this session, we transitioned from manual robot control to full autonomy using ROS 2.

- **Recap:**  
  We began by reviewing how we created a digital twin of our robot, set up hardware interfaces with `ros2_control`, and used teleoperation for manual control in both simulation and on real hardware.

- **Sensor Integration:**  
  We introduced LIDAR as the robot’s primary sensor for perceiving its environment, and discussed how ROS enables seamless integration of both real and simulated sensors by publishing standardized data topics.

- **SLAM (Simultaneous Localization and Mapping):**  
  We explored the SLAM problem—how a robot builds a map of an unknown environment while localizing itself within it. Using the `slam_toolbox` package, we combined LIDAR and odometry data to create a map and correct for drift, enabling reliable navigation.

- **Autonomous Navigation with Nav2:**  
  With mapping and localization in place, we leveraged the Nav2 stack for autonomous navigation. Nav2 plans safe paths to user-defined goals and sends velocity commands to the robot, using the same interfaces established for manual control.

- **System Integration:**  
  We visualized the complete ROS system graph, showing how all nodes—from sensors to actuators—interact in the autonomy pipeline.

- **Assignment:**  
  You will integrate these components to achieve autonomous navigation in simulation, demonstrating your robot navigating to a goal and submitting your results.

- **Next Steps:**  
  We concluded by highlighting future directions, such as advanced perception, manipulation, and custom behaviors in ROS.

This session built a solid foundation for understanding and implementing autonomous navigation in mobile robots using ROS 2.

## 🎓 Capstone Project - Part 2

### 🛠️ Development Environment Setup (Pre-requisite)

Before proceeding with the robot setup, complete the following:

1. Run the installation steps provided here:  
   👉 https://github.com/soham2560/ros2_tutorial_repo

2. Pull the Docker image:
   ```bash
   docker pull ghcr.io/soham2560/humble-garden:latest
    ```
    📦 Image link: [humble-garden container](https://github.com/soham2560/DockerForROS2Development/pkgs/container/humble-garden)

### 🚀 Autonomous Robot Navigation

Choose **one** of the following repositories and follow the instructions to set up your development environment and launch the robot in simulation and real-life:

- [HepoBot GitHub Repository](https://github.com/rtarun1/HepoBot)  
- [MecaBot GitHub Repository](https://github.com/soham2560/MecaBot)

### 🎯 Goal
Successfully launch the robot, integrate the provided autonomy stack (including LIDAR, SLAM, and Nav2), and demonstrate autonomous navigation in simulation.

---

## 🔗 Resources

| Topic/Tool                         | Link                                                                                                                                      |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| 📑 Lecture Slides – ROS Deployment 2 | [![PDF](https://img.shields.io/badge/Open-Slides-red?logo=adobeacrobatreader&logoColor=white)](./lec-21-ros-deployment-2.pdf)            |
| 📘 Articulated Robotics Tutorials     | [![Visit](https://img.shields.io/badge/Open-Tutorials-brightgreen?logo=readthedocs&logoColor=white)](https://articulatedrobotics.xyz/tutorials/) |
| 📚 Nav2 Documentation                 | [![Docs](https://img.shields.io/badge/Open-Nav2%20Docs-blueviolet?logo=ros&logoColor=white)](https://docs.nav2.org)                      |
| 🏗️ Gazebo Getting Started             | [![Docs](https://img.shields.io/badge/Open-Gazebo-orange?logo=gazebo&logoColor=white)](https://gazebosim.org/docs/latest/getstarted/)   |


