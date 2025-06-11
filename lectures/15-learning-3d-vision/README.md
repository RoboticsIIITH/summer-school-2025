# Lecture 15: Learning for 3D Vision

**Instructor:** Akash Kumbar  
**Date:** June 4, 2025

---

## 📖 Overview

Today’s session was an exploration of how geometry meets learning, diving into representations, processing techniques, and modern neural approaches in **3D vision**.

We began by breaking down the core 3D representations used across research and industry:

* **Point Clouds** for their lightweight, unordered nature.
* **Voxels** as volumetric grids that bridge 2D and 3D intuitions.
* **Meshes** to model surface geometry and topology.
* And the rising trend of **implicit representations**, which bypass discrete geometry altogether by learning continuous functions.


Next, we explored **deep learning** methods tailored to these representations:

* **VoxNet** introduced us to applying CNNs on voxel grids.
* **PointNet** and **PointNet++** revealed how to learn directly from raw point clouds, with increasing locality.
* We wrapped up with **DGCNN**, which brings in dynamic graph structures to model point relationships more richly.

To go deeper into the geometric side, we covered **point cloud processing techniques** — essential for preparing data and improving learning robustness:

* **Poisson Disk Sampling** for uniform sub-sampling without clumping.
* **Farthest Point Sampling (FPS)** as a greedy but effective strategy for downsampling with maximal coverage.
* And a few other tricks of the trade to make point clouds more learnable.

Finally, we zoomed out to **novel view synthesis** representations with **Neural Radiance Fields (NeRFs)**, a breakthrough in 3D scene reconstruction using implicit volumetric rendering that synthesizes novel views with remarkable photorealism. We wrapped up by introducing **3D Gaussian Splatting**, a fast and efficient alternative that models scenes with **ellipsoid-based representations**, enabling real-time rendering with high visual fidelity.

All in all, the session connected the dots from classical geometric representations to the neural pipelines that now define modern 3D vision.

---

## 📄 Hands-On Workbooks

| Topic                         | Notebook                                                                                  |
|------------------------------|-------------------------------------------------------------------------------------------|
| **VoxNet (Intro to 3D CNNs)** | [![Open in Colab](https://img.shields.io/badge/Open%20in-Colab-orange?logo=google-colab&logoColor=white)](https://colab.research.google.com/drive/1Lta7m7rvhX7W4Wiv7QYJBDLB0HbLg4Iw?usp=sharing) |
| **PointNet**                 | [![Open in Colab](https://img.shields.io/badge/Open%20in-Colab-orange?logo=google-colab&logoColor=white)](https://colab.research.google.com/drive/1W4EZv0kabfGZ9orbHpWXqXEaHaaqM-hV?usp=sharing) |
| **PointNet++**               | [![Open in Colab](https://img.shields.io/badge/Open%20in-Colab-orange?logo=google-colab&logoColor=white)](https://colab.research.google.com/drive/117O7VN24Ibonp3fg2F1Sr5vgKZXMl5-P?usp=sharing) |

👇 Do also go through all the listed resources below.

📣 Please submit any questions or discussion points on the **`#module-4-multiview-geometry`** Slack channel.

---

## 🔗 Resources

| 📚 Topic                                                             | 🔗 Link                                                                                                                                                            |
|----------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 📑 Lecture Slides – 3D Vision                            | [![PDF](https://img.shields.io/badge/Open-Slides-red?logo=adobeacrobatreader&logoColor=white)](./lec-15-3d-vision.pdf)                    |
| 🎓 Course – Geometry Processing (École Polytechnique)               | [![Course Website](https://img.shields.io/badge/View-Course%20Page-blue?logo=Google%20Classroom&logoColor=white)](https://www.lix.polytechnique.fr/~maks/Verona_MPAM/schedule.html)     |
| 🎥 Overview on Digital Geometry Processing - Prof. Keenan Crane (YouTube)                          | [![YouTube](https://img.shields.io/badge/Watch-Overview-red?logo=youtube)](https://www.youtube.com/watch?v=BwpEoZYcrwY)                                           |
| 🎥 Shape Analysis – MIT 6.838 by Justin Solomon (Spring 2021)       | [![YouTube](https://img.shields.io/badge/Watch-Shape%20Analysis-red?logo=youtube)](https://www.youtube.com/playlist?list=PLQ3UicqQtfNtUcdTMLgKSTTOiEsCw2VBW)      |
| 🎥 Gaussian Splatting – Core Algorithm Explanation                  | [![YouTube](https://img.shields.io/badge/Watch-Core%20Algorithm-red?logo=youtube)](https://www.youtube.com/watch?v=2SQUMYw0h0A&ab_channel=xoft)                   |
| 🎥 Gaussian Splatting – Detailed Overview                           | [![YouTube](https://img.shields.io/badge/Watch-Detailed%20Overview-red?logo=youtube)](https://www.youtube.com/watch?v=K0RRdHVU1bU&ab_channel=MinhyukSung)         |
| 🎥 History of 3D Gaussian Splatting (3DGS)                           | [![YouTube](https://img.shields.io/badge/Watch-3DGS%20History-red?logo=youtube)](https://www.youtube.com/watch?v=DjOqkVIlEGY&t=1209s&ab_channel=MatthiasNiessner) |
|🎓 Course – Machine Learning for Inverse Graphics by Prof. Vincent Sitzmann (Spring 2023) | [![Course Website](https://img.shields.io/badge/View-Course%20Page-blue?logo=Google%20Classroom&logoColor=white)](https://www.scenerepresentations.org/courses/2023/fall/inverse-graphics/) |

