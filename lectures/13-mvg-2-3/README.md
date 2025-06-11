# Lecture 13: Multi-View Geometry - II, III

**Instructor:** Rohit  
**Date:** June 2, 2025 (☀️ Afternoon Session)

---
## 📖 Overview

This session extended our foundational understanding of multiple-view geometry by addressing how cameras relate across different viewpoints — a crucial building block for structure-from-motion, visual odometry, and SLAM systems.

We began by revisiting the core mathematical tool of **homographies**, which capture planar transformations between views. This naturally led to a study of **Zhang’s method** for camera calibration using homographies, offering a practical route to estimate intrinsic parameters from multiple images of a known planar scene.

To handle noisy correspondences and outliers, we introduced **RANSAC** — a robust estimation framework critical for real-world matching tasks. With this in place, we explored **local feature matching**, comparing classical methods like **SIFT with Lowe’s ratio test** to modern **deep learning-based descriptors** such as **SuperPoint**, **SuperGlue**, and **LoFTR**. The transition from handcrafted to learned representations highlights a shift toward end-to-end optimized pipelines in vision.

We then studied **Perspective-n-Point (PnP)** problems and compared them with the **Direct Linear Transform (DLT)**. While DLT applies to general projection problems using 2D–3D correspondences (with unknow intrinsics), PnP specifically estimates camera pose (given intrinsics) from known 3D landmarks and their image projections — a key subroutine in visual localization.

### 🧩 Self-Study Extensions

To further reinforce the geometry between views, we encourage self-study on (resources provided below):

- The **Fundamental Matrix**, its geometric meaning, and estimation via the **8-point algorithm**.
- The **Essential Matrix**, and its decomposition to recover relative rotation and translation between cameras.
- **Monocular Visual Odometry**, showing how sequential pose estimation can be achieved using only a single moving camera.

Each of these topics builds upon the previous, forming a coherent pipeline from calibration to correspondence to motion — essential for any modern vision or robotics system.

---

## 📄 Assignments:

- 📘 **Monocular Visual Odometry:** [![PDF](https://img.shields.io/badge/Open-Problem%20Set%20PDF-red?logo=adobeacrobatreader&logoColor=white)](./visual_odometry_problem_set.pdf)  
 
  Implement a full **monocular visual odometry pipeline** on a short KITTI sequence. The steps include:
  1. Estimating the **Fundamental Matrix** using the **8-point algorithm**.
  2. Computing the **Essential Matrix** using the known intrinsic calibration matrix **K**.
  3. **Recovering relative rotation and translation (R, t)** from the Essential Matrix.
  4. **Comparing the estimated trajectory** with the ground truth using **`evo_ape`** or other trajectory evaluation tools.

- 📘 **Visual Features (From Classical to Deep Learning):** [![Open in Colab](https://img.shields.io/badge/Open%20in-Colab-orange?logo=google-colab&logoColor=white)](https://colab.research.google.com/drive/1NPN8j9mH9b2eiZPVPJRF8-T2OOuwWwxy?usp=sharing)

  This notebook guides you through the evolution of keypoint-based feature extraction and matching:
  1. Classical methods including **Shi-Tomasi** and the **Harris Corner Detector**.
  2. Scale-invariant features using **SIFT** with **Lowe’s ratio test**.
  3. Deep learning-based matchers such as **SuperPoint**, **SuperGlue**, and **LoFTR** — highlighting modern, robust alternatives for correspondence estimation.
  
  _Courtesy: Kumaraditya_
  


💬 Post any questions or progress updates in the **`#module-4-multiview-geometry`** Slack channel.


## 🔗 Resources

| Topic                                                | Link                                                                                     |
|------------------------------------------------------|------------------------------------------------------------------------------------------|
| **Lecture Slides - Homography, PnP, Triangulation** | [lec-13-mvg-homography-pnp-triangulation.pdf](./lec-13-mvg-homography-pnp-triangulation.pdf) |
| **Mobile Sensing & Robotics II - Cyrill Stachniss** *(Playlist)* | [![YouTube](https://img.shields.io/badge/YouTube-MSR_II_Playlist-red?logo=youtube)](https://www.youtube.com/watch?v=mQvKhmWagB4&list=PLgnQpQtFTOGQh_J16IMwDlji18SWQ2PZ6) |
| Zhang’s Method and P3P *(Lectures 29–31)*              | [![YouTube](https://img.shields.io/badge/YouTube-Lectures_29_–_31-red?logo=youtube)](https://www.youtube.com/watch?v=z92eUJjIJeY&list=PLgnQpQtFTOGQh_J16IMwDlji18SWQ2PZ6&index=32) |
| Fundamental and Essential Matrix Intro *(Lec 32)*      | [![YouTube](https://img.shields.io/badge/YouTube-Lecture_32-red?logo=youtube)](https://www.youtube.com/watch?v=z92eUJjIJeY&list=PLgnQpQtFTOGQh_J16IMwDlji18SWQ2PZ6&index=32) |
| Relative Orientation and F, E Properties *(Lec 33)*    | [![YouTube](https://img.shields.io/badge/YouTube-Lecture_33-red?logo=youtube)](https://www.youtube.com/watch?v=z92eUJjIJeY&list=PLgnQpQtFTOGQh_J16IMwDlji18SWQ2PZ6&index=33) |
| Epipolar Geometry Construction *(Lec 35)*              | [![YouTube](https://img.shields.io/badge/YouTube-Lecture_35-red?logo=youtube)](https://www.youtube.com/watch?v=z92eUJjIJeY&list=PLgnQpQtFTOGQh_J16IMwDlji18SWQ2PZ6&index=35) |
| Estimating F, E (8-Point & Nister’s 5-Point) *(Lec 36–37)* | [![YouTube](https://img.shields.io/badge/YouTube-Lectures_36_–_37-red?logo=youtube)](https://www.youtube.com/watch?v=z92eUJjIJeY&list=PLgnQpQtFTOGQh_J16IMwDlji18SWQ2PZ6&index=36) |
| **PnP: Perspective-n-Point Problem – Steven LaValle (NPTEL)** | [![YouTube](https://img.shields.io/badge/YouTube-Lecture_49-red?logo=youtube)](https://www.youtube.com/watch?v=0JGC5hZYCVE&list=PLbMVogVj5nJSyt80VRXYC-YrAvQuUb6dh&index=50) |

---

