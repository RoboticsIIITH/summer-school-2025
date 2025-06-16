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
- **Green-Board Homework Problems:**
    1. $\frac{\partial^2 f}{\partial x_1 \partial x_2} \overset{?}{=} \frac{\partial^2 f}{\partial x_2 \partial x_1}$

    2. MIT – Matrix Calculus (Edelman OCW)  
    Watch: [Matrix Calculus for Machine Learning (IAP 2023)](https://ocw.mit.edu/courses/18-s096-matrix-calculus-for-machine-learning-and-beyond-january-iap-2023/)

    3. Let $f(x) = \|x\|_2$ (i.e., L2 norm).  
    Compute or reason about: $\nabla f(x)\ ?$  
    (Hint: Try expressing $\|x\|_2 = \sqrt{x^T x}$)

    4. Affine Functions  
    Review definition and properties.

    5. KKT Conditions  
    Recall the general form and interpret geometrically.

    6. Optimization Problem: Let $f(x, y) = x + y$.  
       Minimize it subject to the constraint: $x^2 + y^2 = 4$.

    7. Why is $-\nabla f(x)$ the direction of **steepest descent**?

    8. LM Method (Levenberg–Marquardt)  
    Go through a derivation or interpretation of its update step.

Please submit questions or discussion points on the **`#module-1-math-background`** Slack channel.

---

## 🔗 Resources

| Topic                             | Link                                                                                   |
|----------------------------------|----------------------------------------------------------------------------------------|
| Lecture Notes             | [lec-04-nlopt-notes.pdf](./lec-04-nlopt-notes.pdf)                    |
| 🧮 Matrix Calculus for Machine Learning – Prof. Edelman (MIT OCW) | [![Website](https://img.shields.io/badge/Open-Course-blue?logo=mit&logoColor=white)](https://ocw.mit.edu/courses/18-s096-matrix-calculus-for-machine-learning-and-beyond-january-iap-2023/) |
| 📘 Robust Optimization for SLAM – Niko Sünderhauf (Section 3.3: NLLS) | [![PDF](https://img.shields.io/badge/Open-Thesis_Section_3.3-blue?logo=adobeacrobatreader&logoColor=white)](https://eprints.qut.edu.au/109667/1/109667.pdf#page=59) |
---

## 🧠 Notes

Optimization is core to robotics — from calibration to motion planning. In SLAM, it's used to **stitch local maps into a globally consistent trajectory** by minimizing pose and landmark errors.

While deep learning relies on **first-order methods** like gradient descent, **second-order methods** such as Gauss-Newton and Levenberg-Marquardt **converge faster** and are crucial in robotics where precision and speed matter.
