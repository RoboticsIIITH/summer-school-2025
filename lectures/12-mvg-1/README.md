# Lecture 12: Multi-View Geometry - I

**Instructor:** Rohit  
**Date:** June 2, 2025 (🌅 Morning Session)

---

## 📖 Overview

In this session, we laid the mathematical and geometric foundations of how cameras capture the world — the first step in many vision and robotics pipelines.

We began with the **geometry of image formation**, focusing on the **pinhole camera model** as the ideal abstraction for understanding how 3D points are projected onto 2D images. This led us to the **perspective projection equation**, which formalizes this mapping using homogeneous coordinates.

From there, we broke down the **projection matrix** — what it encodes, how it's constructed, and how it intertwines the **intrinsic** and **extrinsic** properties of a camera. We explored the **anatomy of the projection matrix** and how it can be **decomposed** to recover meaningful camera parameters.

With this structure in place, we moved into **camera calibration**: the process of estimating camera parameters from known data. We covered **Tsai’s method**, one of the classical approaches, and then focused on the **Direct Linear Transform (DLT)** algorithm — a fundamental technique that frames calibration as a linear system solvable via **SVD**.

Each topic built on the last, tying together geometry, algebra, and practical calibration to help you understand how a robot (or algorithm) begins to make sense of visual input.

---

## 📄 Assignment: Direct Linear Transform (DLT)

- 📘 **Exercise Notebook:** [direct-linear-transform.ipynb](direct-linear-transform.ipynb)  
  Implement the **Direct Linear Transform (DLT)** algorithm on images of a **Rubik’s Cube** to estimate camera projection.

💬 Please post any questions or discussion points in the **`#module-4-multiview-geometry`** Slack channel.

---

## 🔗 Resources

| Topic                                                | Link                                                                                     |
|------------------------------------------------------|------------------------------------------------------------------------------------------|
| **Lecture Slides - Camera Modeling, Camera Calibration** | [lec-12-mvg-camera-calibration.pdf](./lec-12-mvg-camera-calibration.pdf) |
| **Mobile Sensing & Robotics II – Cyrill Stachniss (2021)** *(Lectures 23–27: Camera Parameters & DLT)* | [![YouTube](https://img.shields.io/badge/YouTube-Lectures_23–27-red?logo=youtube)](https://www.youtube.com/watch?v=ND2fa08vxkY&list=PLgnQpQtFTOGQh_J16IMwDlji18SWQ2PZ6&index=23) |
| **First Principles of Computer Vision – Shree K. Nayar** *(Channel)* | [![YouTube](https://img.shields.io/badge/YouTube-Shree_K._Nayar_Channel-red?logo=youtube)](https://www.youtube.com/@firstprinciplesofcomputerv3258) |
| Image Formation *(Playlist)*                                     | [![YouTube](https://img.shields.io/badge/YouTube-Image_Formation-red?logo=youtube)](https://www.youtube.com/watch?v=_QjxbQKY4ds&list=PL2zRqk16wsdr9X5rgF-d0pkzPdkHZ4KiT) |
| Camera Calibration *(Playlist)*                                  | [![YouTube](https://img.shields.io/badge/YouTube-Camera_Calibration-red?logo=youtube)](https://www.youtube.com/watch?v=S-UHiFsn-GI&list=PL2zRqk16wsdoCCLpou-dGo7QQNks1Ppzo) |
| **Computer Vision – Andreas Geiger (Uni Tübingen)** *(Course + Playlist)* | [![YouTube](https://img.shields.io/badge/YouTube-Playlist-red?logo=youtube)](https://www.youtube.com/watch?v=YW1cIaOBkI8&list=PL05umP7R6ij35L2MHGzis8AEHz7mg381_) [![Website](https://img.shields.io/badge/Site-Course_Page-grey?logo=google-chrome)](https://uni-tuebingen.de/fakultaeten/mathematisch-naturwissenschaftliche-fakultaet/fachbereiche/informatik/lehrstuehle/autonomous-vision/lectures/computer-vision/) |
| Lecture 02: Image Formation *(Slides)*                           | [![Drive](https://img.shields.io/badge/Slides-Image_Formation-blue?logo=google-drive)](https://drive.google.com/file/d/1UfcxEkqoXkHgOCZpUnzRHn7NM2hTqd38/view?usp=sharing) |
| 📷 Cameras and Lenses – Interactive Visual Explainer by Bartosz Ciechanowski | [![Website](https://img.shields.io/badge/Open-Demo-blue?logo=googlechrome&logoColor=white)](https://ciechanow.ski/cameras-and-lenses/) |
---

