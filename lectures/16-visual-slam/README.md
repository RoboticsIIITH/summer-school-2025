# Lecture 16: Visual SLAM

**Instructor:** Aneesh  
**Date:** June 5, 2025

---

📖 Overview

Today’s session introduced the foundations of **Simultaneous Localization and Mapping (SLAM)** — the core capability that allows robots to **build a map of an unknown environment while simultaneously estimating their own pose** within it.

We began by discussing the inherent circular dependency at the heart of SLAM: **localization requires a map, and mapping requires localization**. SLAM solves this interdependence by treating both as a joint optimization problem using sensor constraints from cameras, IMUs, LiDARs, and more.

We introduced the concept of **pose graphs**, where **nodes represent poses** and **edges represent sensor-derived constraints** (like odometry or loop closures). Optimization libraries such as **G2O** refine the entire graph to reduce drift and improve consistency.

A toy **1D SLAM example** helped illustrate how **landmarks and loop closures act as constraints**. As drift accumulates over time, closing a loop enables the system to back-propagate corrections through the graph, significantly improving trajectory accuracy.

In the real world, SLAM powers everything from **search and rescue operations** and **warehouse automation** to **consumer robots** and **AR/VR experiences**, where robust and efficient localization is key.

We also reviewed various **sensor configurations and SLAM systems**: from monocular methods like **ORB-SLAM2**, RGB-D systems like **ElasticFusion**, LiDAR-based techniques like **LOAM**, to tightly-coupled visual-inertial odometry systems like **VINS-Fusion** and **LIO-SAM**.

Despite its promise, SLAM faces several challenges: **sensor noise**, **drift accumulation**, **false loop closures**, **real-time constraints**, and **long-term consistency** in dynamic environments.

Altogether, this session offered a foundational lens into how SLAM frameworks are built, what sensors and algorithms they depend on, and how they scale from academic demos to real-world autonomy.


---

## 📄 Assignment
🛠️ **Hackable 3D Instance Mapping Setup**:

- We'll set up [**Concept Nodes**](https://github.com/sachaMorin/concept-nodes), a lightweight re-implementation of [ConceptGraphs](https://concept-graphs.github.io/) by one of the original authors, **Sacha Morin**. Explore the repository by trying out different configurations and graph-building options.

- Your goal is to understand how the framework attempts **3D instance mapping** from RGB-D streams and investigate ways to improve robustness for **indoor semantic mapping**. Think about potential extensions, better descriptors, or improved spatial consistency strategies.

- Understand various **evaluation metrics** (how are the AP, AP25, AP50 metrics calculated) used to assess mapping quality, such as **semantic consistency** and **instance accuracy** — refer to the [ScanNet Benchmark](https://kaldir.vc.in.tum.de/scannet_benchmark/semantic_instance_3d) and the [ConceptGraphs evaluation discussion](https://github.com/concept-graphs/concept-graphs/issues/18#issuecomment-1876673985) for details. Implement an evaluation script for ConceptNodes along these metrics.


## 🔗 Resources
| 📚 Topic                                | 🔗 Link                                                                                                                                       |
|-----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| 📑 Lecture Slides – Visual SLAM                          | [![PDF](https://img.shields.io/badge/Open-Slides-red?logo=adobeacrobatreader&logoColor=white)](./lec-16-visual-slam.pdf)                    |
| 🎥 Basics of SLAM – Cyril Stachniss     | [![YouTube](https://img.shields.io/badge/Watch-YouTube-red?logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PLgnQpQtFTOGQrZ4O5QzbIHgl3b1JHimN_) |
| 📦 RTAB-Map                             | [![Website](https://img.shields.io/badge/Open-rtabmap-blue?logo=github&logoColor=white)](http://introlab.github.io/rtabmap/)                |
| 🧠 Concept Graphs                       | [![Website](https://img.shields.io/badge/Open-concept--graphs-green?logo=github&logoColor=white)](https://concept-graphs.github.io/)        |
| ⚙️ g2o – Graph Optimization             | [![GitHub](https://img.shields.io/badge/View-g2o-181717?logo=github)](https://github.com/RainerKuemmerle/g2o)                                |
| ⚙️ Ceres Solver                         | [![Website](https://img.shields.io/badge/Open-ceres--solver-9cf?logo=google&logoColor=white)](http://ceres-solver.org/)                      |
| 📖 The SLAM Handbook | [![GitHub](https://img.shields.io/badge/View-SLAM%20Handbook-181717?logo=github)](https://github.com/SLAM-Handbook-contributors/slam-handbook-public-release) |
| 📖 14 Lectures on Visual SLAM by Gao Xiang <br> (with C++ Impl.)         | [![GitHub](https://img.shields.io/badge/View-on%20GitHub-blue?logo=github)](https://github.com/gaoxiang12/slambook-en)                     |


> 🚀 **Recommended Reading: [The SLAM Handbook](https://github.com/SLAM-Handbook-contributors/slam-handbook-public-release)**  
> An open-access, very up-to-date textbook **authored by leading experts in the SLAM community**. Must read for anyone into perception for robotics!  


