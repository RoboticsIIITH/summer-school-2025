# Lecture 14: Multi-View Geometry - IV

**Instructor:** Rohan  
**Date:** June 03, 2025

---

## 📖 Overview

We started off with a description of the **Structure from Motion (SfM)** task, and how **Bundle Adjustment** serves as the optimization method to solve this problem. We then moved into a detailed breakdown of the task — what parameters are involved and how the loss function is formulated.

Next, we discussed the issues with using a **Homogeneous Coordinate System**, particularly the ambiguity introduced by scale. We then saw how moving to the **Euclidean Coordinate System** helps resolve this by eliminating scale parameters.

We briefly touched upon **Lie Algebra** — a mathematical framework for 3D transformations that is especially useful for optimization of transformation matrices. Further reading resources have been provided for those interested.

We also explored open-source pipelines for tackling this task:  
- **COLMAP** for solving the core `SfM` pipeline, and  
- **HLoc** as an application layer for relocalization from arbitrary images using a pre-computed `SfM` map.

Finally, we wrapped up by looking at some **deep learning-based approaches** to 3D reconstruction — **DUSt3R** and **MASt3R** — discussing the differences between the two, and how they can be used for both `Reconstruction` and `Re-localization`.


---

## 📄 Assignments

1. 📘 **COLMAP & HLoc Walkthrough:**  
   Open the following notebook for a guided exercise on classical structure-from-motion and local feature-based localization:  
   [![Jupyter](https://img.shields.io/badge/Open%20Notebook-sfm--colmap--hloc.ipynb-orange?logo=jupyter)](./sfm-colmap-hloc.ipynb)

   - Run COLMAP on the *South Building* dataset to generate a sparse 3D model. Try exporting the outputs (`images.txt`, `points3D.txt`, `cameras.txt`).
   - Follow the instructions for HLoc to try out local feature-based localization on the *Sacre Coeur* dataset.

2. 🚀 **MASt3R-based Map-Free Visual Localization Pipeline:**  
   Set up [**MASt3R**](https://github.com/naver/mast3r) and build a simple map-free visual localization system using your own data.

   **Steps:**
   - **Data Collection**: Use a dataset or collect data using tools like [MARS Logger](https://github.com/OSUPCVLab/mobile-ar-sensor-logger). Create two runs:  
     - A **reference run** (serving as the map).  
     - A **query run** (frames to localize).
   - **Image Retrieval**: For each query frame, retrieve top matching reference frames using [HLoc](https://github.com/cvg/Hierarchical-Localization).  
     (Tip: `CosPlace` works well for indoor scenes.)
   - **Feature Matching**: Run matching between retrieved reference and query frames.
   - **3D Lifting**: Project the matched keypoints in the reference images into 3D using MASt3R’s predicted depth/pointmap.
   - **Pose Estimation**: Use the 2D-3D matches to estimate pose using **PnP**.
   - **Evaluation**: Plot the estimated query trajectory and compare it to ground truth using [`evo`](https://github.com/MichaelGrupp/evo).
   - **Bonus / Studies**  
  What other options are available for image retrieval — can the features from **MASt3R** itself be repurposed for this task? For relative pose estimation, could one use the **Essential Matrix** instead of PnP, and under what conditions would it be preferable? Evaluate how well MASt3R estimates depth maps: how does it compare to sensor-based depths? You could also try using [**UniDepthV2**](https://github.com/lpiccinelli-eth/UniDepth) or [**Metric3Dv2**](https://github.com/YvanYin/Metric3D) to estimate depth and compare their predictions with MASt3R's outputs.



📣 All necessary repositories have been linked in the slides. Post your progress or questions on the `#module-4-multiview-geometry` Slack channel!

---

## 🔗 Resources


| Topic                                  | Link |
|---------------------------------------------------------|------|
| 📑 Lecture Slides – Structure-from-Motion & 3D Foundation models  | [lec-14-sfm.pdf](./lec-14-sfm.pdf) |
| Short Introduction to the SFM Problem         | [![YouTube](https://img.shields.io/badge/YouTube-Intro-red?logo=youtube)](https://www.youtube.com/watch?v=JlOzyyhk1v0&pp=ygUiY3lyaWxsIHN0YWNobmlzcyBidW5kbGUgYWRqdXN0bWVudA%3D%3D) |
| Basics of Bundle Adjustment – Cyrill Stachniss   | [![YouTube](https://img.shields.io/badge/YouTube-BA_Basics-red?logo=youtube)](https://www.youtube.com/watch?v=sobyKHwgB0Y&t=104s&pp=ygUiY3lyaWxsIHN0YWNobmlzcyBidW5kbGUgYWRqdXN0bWVudA%3D%3D) |
| Numerics of Bundle Adjustment – Cyrill Stachniss | [![YouTube](https://img.shields.io/badge/YouTube-BA_Numerics-red?logo=youtube)](https://www.youtube.com/watch?v=LKDLcKrWOIU&pp=ygUiY3lyaWxsIHN0YWNobmlzcyBidW5kbGUgYWRqdXN0bWVudA%3D%3D) |
| Lecture Slides – Levenberg–Marquardt (courtesy Gnana Prakash) | [![PDF](https://img.shields.io/badge/PDF-levenberg--marquadt-blue?logo=adobeacrobatreader)](./levenberg-marquadt.pdf) |
| 📑 Slides – ICP SLAM with Lie Theory (courtesy Shubodh Sai)    | [![PDF](https://img.shields.io/badge/PDF-icp--slam--shubodh-blue?logo=adobeacrobatreader)](./icp-slam-shubodh.pdf) |
| 📖 Karnik Ram’s Blog on Lie Groups and Lie Algebra               | [![Blog](https://img.shields.io/badge/Read-Blog-orange?logo=readthedocs)](https://karnikram.info/blog/lie/) |
| 📘 Optimization on Manifolds – José Luis Blanco Claraco          | [![arXiv](https://img.shields.io/badge/arXiv-2103.15980-b31b1b?logo=arxiv)](https://arxiv.org/abs/2103.15980) |
| 📘 Chapter 3 – Lie Groups and Algebra from SLAM Book            | [![PDF](https://img.shields.io/badge/Read-SLAM_Book_Chapter_3-blue?logo=readthedocs)](https://github.com/gaoxiang12/slambook-en/blob/master/slambook-en.pdf) |


> More resources are available inline with the slides - do check them out!
---