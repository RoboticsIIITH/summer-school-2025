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
---