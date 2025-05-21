# Lecture 04: Non-Linear Optimization

**Instructor:** Faizal  
**Date:** May 21, 2025

---

## 📖 Overview

This lecture explores the fundamentals of optimization with a focus on non-linear systems. We begin by revisiting vector derivatives, gradients, and Hessians, and how they inform optimization landscapes. Key distinctions between linear and non-linear equations will be drawn, particularly in the context of error modelling.

We then dive into constrained optimization via Lagrange Multipliers and discussed both analytical (closed-form) and iterative approaches. The session concludes with foundational methods for solving non-linear least squares problems, including **Gradient Descent**, **Gauss-Newton**, and the **Levenberg-Marquardt algorithm**, all of which are vital tools in robotics and computer vision.

---

## 📄 Assignment

- **Exercise Notebook:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1KoL1K9w3FtYSm9gJYajri4OdVuCEhC7x?usp=sharing)

Please submit questions or discussion points on the **`#module-1-math-background`** Slack channel.

---

## 🔗 Resources

| Topic                             | Link                                                                                   |
|----------------------------------|----------------------------------------------------------------------------------------|
| Lecture Notes             | [lec-04-nlopt-notes.pdf](./lec-04-nlopt-notes.pdf)                    |

---

## 🧠 Notes

Optimization is core to robotics — from calibration to motion planning. In SLAM, it's used to **stitch local maps into a globally consistent trajectory** by minimizing pose and landmark errors.

While deep learning relies on **first-order methods** like gradient descent, **second-order methods** such as Gauss-Newton and Levenberg-Marquardt **converge faster** and are crucial in robotics where precision and speed matter.
