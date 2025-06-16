# Lecture 06: Dynamics and Control - II

**Instructors:** Sarthak, Astik  
**Date:** May 23, 2025

---

## 📖 Overview

### 🎛️ Control Systems

We introduce the structure and intent of control in robotics:

- **Hierarchies of control**: from strategic planning to real-time actuation.
- **Anatomy of a control loop**: sensing, decision, and execution.
- **Where control matters**: trajectory tracking, stabilization, interaction, and more!

We then transition into key techniques and applications in modern control:

- **PID Control**  
  One of the most widely used feedback control methods. We study the role of proportional, integral, and derivative components in correcting system behavior. Examples include motor speed regulation and balancing systems.

- **Control Loops in Aerial Vehicles**  
  We dissect the layered architecture of drone and aircraft control systems:
  - *L1 Controller*: guides high-level navigation (e.g., path following).
  - *Attitude Controller*: manages the vehicle’s orientation.
  - *TECS (Total Energy Control System)*: balances throttle and pitch to manage altitude and speed in fixed-wing aircraft.

- **Optimal Control - LQR (Linear Quadratic Regulator)**  
  We introduce the idea of designing a controller that minimizes a quadratic cost function over time. LQR provides a principled way to balance control effort against system performance, and is especially useful for linear systems with state-space representations.

Together, these topics build a foundation for understanding both classical and modern control strategies used in robotics and autonomous systems.

---

## 📄 Assignment

- **Exercise Notebooks:** TBD

Please raise doubts or engage in discussion on the **`#module-2-dynamics-control`** Slack channel.

---

## 🔗 Resources

| Topic                             | Link                                                                                   |
|----------------------------------|----------------------------------------------------------------------------------------|
| Lecture Slides (Sarthak) - Controls - Introduction         | [lec-06-controls-introduction.pdf](./lec-06-controls-introduction.pdf)                    |
| Lecture Slides (Astik) - Controls - PID, LQR        | [lec-06-controls-pid-lqr.pdf](./lec-06-controls-pid-lqr.pdf)                  |
| **Modern Robotics: Mechanics, Planning, and Control** – Kevin M. Lynch & Frank C. Park (Northwestern University) | [![Textbook](https://img.shields.io/badge/Open-Textbook-blue?logo=readthedocs)](https://hades.mech.northwestern.edu/index.php/Modern_Robotics)<br>[![Videos](https://img.shields.io/badge/Watch-Lecture_Videos-red?logo=youtube&logoColor=white)](https://hades.mech.northwestern.edu/index.php/Modern_Robotics_Videos) |
| **Computational Control** (Saverio Bolognani, ETH Zurich, 2024) | [![Course Website](https://img.shields.io/badge/View-Course_Website-brightgreen?logo=academia)](https://www.bsaver.io/teaching/computational-control)<br>[![Chat with COCO Expert](https://img.shields.io/badge/Chat-🥥%20COCO%20Expert-brown?style=flat&labelColor=white)](https://bsaver.io/COCO-Expert) |

---