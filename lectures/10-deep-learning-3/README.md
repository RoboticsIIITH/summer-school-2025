# Lecture 10: Deep Learning - III

**Instructors:** Swayam, Vansh  
**Date:** May 28, 2025

---

## 📖 Overview

In this session, we began by introducing the **basics of image descriptors**, highlighting traditional techniques like **SIFT** for keypoint detection, feature extraction, and matching across images. This provided historical context for how machines interpret visual data before deep learning.

We then transitioned into **Convolutional Neural Networks (CNNs)**, exploring their architecture and core building blocks:
- **Convolution operations** for local feature extraction  
- **Pooling layers** for spatial downsampling  
- **Activation functions** for introducing non-linearity

We discussed the challenges of **vanishing and exploding gradients**, particularly in deep architectures, and how they hinder effective learning during backpropagation. This naturally led into **Residual Networks (ResNets)** and their innovative use of **skip connections** to enable training of very deep networks by preserving gradient flow.

Finally, we explored **Transfer Learning** and **Fine-Tuning**, two powerful strategies for leveraging pretrained models:
- **Transfer Learning**: Using CNNs trained on large datasets (e.g., ImageNet) as feature extractors  
- **Fine-Tuning**: Updating selected layers to adapt the model to a new task

Together, these concepts build a solid intuition for how deep learning models process and understand visual data.

---

## 📄 Assignment

- **Exercise Notebook:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/18txr34ybFEwosnieoRhWLT6hgZ204_wL)

Please submit any questions or discussion points on the **`#module-3-deep-learning`** Slack channel.

---

## 🔗 Resources

| Topic                                                | Link                                                                                     |
|------------------------------------------------------|------------------------------------------------------------------------------------------|
| Lecture Slides - Deep Learning - CNNs | [lec-10-dl-cnns.pdf](./lec-10-dl-cnns.pdf) <br> [![View in Google Slides](https://img.shields.io/badge/View-Google%20Slides-4285F4?logo=google-slides&logoColor=white)](https://docs.google.com/presentation/d/1mhSJ4OA4Q9CVvM_LYre3Io19rLexaTKQ6nt39ZNIKLQ/edit?usp=sharing) |
| CNN Interactive Visualization                        | [CNN Explainer](https://poloclub.github.io/cnn-explainer/)                              |
| CNNs with Multiple Channels                          | [D2L.ai: Channels in CNNs](https://d2l.ai/chapter_convolutional-neural-networks/channels.html) |
| CNN Backpropagation                                  | [CMU Recitation 5: CNN Backprop](https://deeplearning.cs.cmu.edu/F21/document/recitation/Recitation5/CNN_Backprop_Recitation_5_F21.pdf) |
| ResNet Skip Connections (Backpropagation)            | [StackExchange: Backprop through ResNets](https://stats.stackexchange.com/questions/268820/gradient-backpropagation-through-resnet-skip-connections) |
| Loss Landscape Visualization                         | [Loss Landscape Discussion](https://jtuckerk.github.io/loss_landscape.html)             |
| Transposed Convolutions                              | [YouTube: Andrew Ng on Transposed Convolutions](https://www.youtube.com/watch?v=qb4nRoEAASA) |
| Transfer Learning Overview                           | [CS231n: Transfer Learning](https://cs231n.github.io/transfer-learning/)                |
| Transfer Learning Slides                             | [MLDDS Courseware Slides](https://lisaong.github.io/mldds-courseware/03_TextImage/transfer-learning.slides.html) |

---
