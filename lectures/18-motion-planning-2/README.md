# Lecture 18: Motion Planning - II
**Instructor:** Ansh Chablani  
**Date:** June 10, 2025 (🌅 Morning Session)

## Topics Covered:

1. Uncertainty Quantification
2. Parametric/Non-parametric Assumptions 
3. Optimization-based planners
4. CEM and MPC

## Overview

In this lecture, we begun by discussing the various uncertainties in robot motion planning and how things are different in simulation as opposed to in real world.

We discussed several methods to quantify these uncertainties (like robot pose, scene information, etc.) in the real world by using models.

Later, we dived into a fundamental concept in machine learning where a model is classified as parametric or non-parametric depending on whether or not the number of parameters in that model is fixed.
Thereafter, we discussed such ML models used in robot motion planning and classified them as parametric or otherwise.

We discussed optimization as a concept and used it to learn about several optimization based planners like CHOMP and STOMP. Later, we saw some videos which use such planners.

Further, we discussed Cross Entropy Method (CEM) intuitively with a video and explored the math behind it.

Finally, we discussed Model Predictive Control with a diagram and a constructed autonomous car which uses MPC.

Together, these concepts build a solid intuition for some of the motion planning approaches. 

## 🔗 Resources and Interesting Links
| Topic | Link |
|-------|------|
| 📘 A Survey of Optimization-based Task and Motion Planning | [![arXiv](https://img.shields.io/badge/arXiv-2404.02817-b31b1b?logo=arxiv)](https://arxiv.org/abs/2404.02817) |
| 📺 Parametric v/s Non-Parametric ML Algorithms | [![YouTube](https://img.shields.io/badge/YouTube-Parametric_vs_NonParametric-red?logo=youtube)](https://youtu.be/9sEiMp8bCnY?si=Tf12e5Q35cmDKfAF) |
| 📺 CHOMP Optimisation (2D) | [![YouTube](https://img.shields.io/badge/YouTube-CHOMP_2D-red?logo=youtube)](https://youtu.be/41UYgGHGSSo?si=_mUhXQoI_oxFLQNt) |
| 📺 CHOMP (Manipulator) | [![YouTube](https://img.shields.io/badge/YouTube-CHOMP_Manipulator-red?logo=youtube)](https://youtu.be/PTFhdzWlXxI?si=P0qOQHYWkhK2ODDv) |
| 📺 CHOMP (Elevation Map) | [![YouTube](https://img.shields.io/badge/YouTube-CHOMP_Elevation_Map-red?logo=youtube)](https://youtu.be/DX9jTBvWrl8?si=-CCvo6-F8Corcuih) |
| 📺 STOMP | [![YouTube](https://img.shields.io/badge/YouTube-STOMP-red?logo=youtube)](https://youtu.be/KZqi8wAcC4k?si=ep27l2UzpdrOnpfc) |
| 📺 Video Lecture on Optimisation Based Motion Planning | [![YouTube](https://img.shields.io/badge/YouTube-Motion_Planning_Lec-red?logo=youtube)](https://www.youtube.com/watch?v=OjB1fYU-Pvo) |
| 📄 Cross-Entropy Motion Planning | [![PDF](https://img.shields.io/badge/PDF-Ko2012_CE--Motion--Planning-blue?logo=adobeacrobatreader)](https://asco.lcsr.jhu.edu/papers/Ko2012.pdf) |
| 🏎️ Model Predictive Control for Autonomous Racing | [![YouTube](https://img.shields.io/badge/YouTube-MPC_Racing-red?logo=youtube)](https://youtu.be/bjlT-6KVQ7U?si=pdASr991iSrHeuOa) |
| ✍️ "Indeed, I favour MPC over RL" – Yann LeCun | [![Twitter](https://img.shields.io/badge/X-Yann_LeCun_MPC--vs--RL-1DA1F2?logo=x)](https://x.com/ylecun/status/1827787323108393027?lang=en) |
---