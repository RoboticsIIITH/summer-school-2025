# Lecture 11: Deep Learning - IV

**Instructor:** Sanket  
**Date:** May 31, 2025

---

## 📖 Overview

Today’s session was a deep dive into how memory, attention, and self-supervision shape modern deep learning — especially in the context of vision and robotics.

We kicked off with **Recurrent Neural Networks (RNNs)** and their limitations, particularly the *vanishing gradient* problem. This naturally brought us to **LSTMs**, and how their gated architecture offers a workaround by selectively retaining memory. We also saw how *skip connections* show up here too — not just in ResNets.

Building on this, we stepped into **sequence models** like **Seq2Seq** and their role in **neural machine translation**, eventually landing on visual-language grounding via models like *Show, Attend, and Tell*. We connected these to real-world robotics applications, like **temporal point cloud forecasting** using **ATPPNet**.

From there, we pulled back to the bigger picture — transformers. We broke down the core **multi-head attention (MHA)** mechanism, the computational overhead, and why it was a breakthrough for NLP. Then we zoomed into how transformers were ported to vision via **ViTs**, and what changed when that happened.

The last leg of the session focused on **self-supervised learning (SSL)** — from **masked autoencoders** to models like **DINO/DINOv2**, **SAM/SAM2**. We also brought it home by showcasing work from our own lab — including **DiffPrompter** and **Revisit Anything** — tying the entire session into a broader narrative about how core DL architectures evolve into systems that perceive, reason, and act in the world.

---

## 📄 Assignment/Hands-on

- **Colab Exercise Notebooks** have been included inline within the lecture slides at relevant points corresponding to key papers and works. These provide hands-on code to accompany the discussed concepts.

Please submit any questions or discussion points on the **`#module-3-deep-learning`** Slack channel.

---

## 🔗 Resources

| Topic                                                | Link                                                                                     |
|------------------------------------------------------|------------------------------------------------------------------------------------------|
| Lecture Slides - Deep Learning - Memory Networks, Transformers | [lec-11-dl-memory-networks.pdf](./lec-11-dl-memory-networks.pdf) |
| Understanding Attention (Video - Pascal Poupart)     | [![YouTube](https://img.shields.io/badge/YouTube-Video-red?logo=youtube)](https://www.youtube.com/watch?v=OyFJWRnt_AY) |
| Illustrated Transformer (Jay Alammar)                | [![Blog](https://img.shields.io/badge/Blog-Jay_Alammar-blue?logo=githubpages)](https://jalammar.github.io/illustrated-transformer/) |
| Seq2Seq and Attention (Lena Voita)                   | [![Blog](https://img.shields.io/badge/Blog-Lena_Voita-blue?logo=githubpages)](https://lena-voita.github.io/nlp_course/seq2seq_and_attention.html) |
| D2L.ai: Attention Mechanisms and Transformers        | [![D2L.ai](https://img.shields.io/badge/D2L-Attention%20%26%20Transformers-1f77b4)](https://www.d2l.ai/chapter_attention-mechanisms-and-transformers/index.html) |
| Video Playlist for Transformers (General Reference)  | [![YouTube](https://img.shields.io/badge/YouTube-Playlist-red?logo=youtube)](https://www.youtube.com/watch?v=dichIcUZfOw&list=PLRgS_r6tnkkhI-q1auABKLfLWG0suOWln) |
| Vision Transformers - ADL4CV Lecture 8               | [![YouTube](https://img.shields.io/badge/YouTube-ADL4CV_Lecture-red?logo=youtube)](https://www.youtube.com/watch?v=1wANXzUISMU&list=PLog3nOPCjKBl8s3Ia4ZtmOEniuYM3pVGQ&index=8) |
| Vision Transformer - Original Paper                  | [![arXiv](https://img.shields.io/badge/arXiv-2010.11929-b31b1b?logo=arxiv)](https://arxiv.org/abs/2010.11929) |
| Alexa Gordic Explains ViT                            | [![YouTube](https://img.shields.io/badge/YouTube-Alexa_Gordic-red?logo=youtube)](https://www.youtube.com/watch?v=j6kuz_NqkG0&list=PLBoQnSflObckGnAS9mXjqCZhg7VTz4x8n&index=3) |
| Transformer United - Stanford Course                 | [![YouTube](https://img.shields.io/badge/YouTube-Stanford_Course-red?logo=youtube)](https://www.youtube.com/playlist?list=PLoROMvodv4rNiJRchCzutFw5ItR_Z27CM) |
| Transformers as GNNs                                 | [![The Gradient](https://img.shields.io/badge/Blog-The_Gradient-purple?logo=readthedocs)](https://thegradient.pub/transformers-are-graph-neural-networks/) |
| Visual Explanation of Multi-Head Attention           | [![Blog](https://img.shields.io/badge/Blog-AI_Summer-blue?logo=githubpages)](https://theaisummer.com/self-attention/) |

---
