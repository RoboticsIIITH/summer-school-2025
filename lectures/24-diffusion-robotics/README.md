# Lecture 24: Diffusion Models for Robotics
**Instructor:** Jayaram Reddy    
**Date:** June 14, 2025

## Topics Covered:
- Why Diffusion for Control
- Diffusion Policies
- Diffusion for Motion Planning, EDMP
- Diffusion for World-Modeling
- Tradeoffs Autoregressive vs Diffusion Models
- Latent Diffusion

## 📄 Assignments

- 🤖 **Diffusion Policy for Robot Manipulation:**  
   Explore how diffusion models can be applied to learn robotic manipulation behaviors, such as pushing, directly from demonstrations.

   - 📓 **Official Colab Notebook:**  
     [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1gxdkgRVfM55zihY9TFLja97cSVZOZq2B?usp=sharing)

   - 🤗 **Hugging Face Playground – Push Task Demo:**  
     [![Open on Hugging Face](https://img.shields.io/badge/Launch-HF_Notebook-blueviolet?logo=huggingface&logoColor=white)](https://huggingface.co/lerobot/diffusion_pusht)

   **What to Do:**
   - Run the official notebook to understand the structure of the Diffusion Policy model and how it leverages conditional generation for trajectory prediction.
   - Try out the push environment on Hugging Face to see the learned policy in action.
   - Reflect on how diffusion-based imitation compares with classical behavioral cloning.
   - (Optional) Try swapping out the dataset or varying inference steps to observe differences in performance.

   > 🧠 This exercise builds intuition for how generative models can drive robotic agents with flexibility and generalization.

📢 Please feel free to post all questions over at the `#module-7-robot-learning` Slack channel.

## 🔗 Resources

| 📚 Topic | 🔗 Link |
|----------|--------|
| 📑 Lecture Slides – Diffusion for Robotics | [![PDF](https://img.shields.io/badge/Open-PDF-red?logo=adobeacrobatreader&logoColor=white)](./lec-24-diffusion-robotics.pdf) [![Slides](https://img.shields.io/badge/Open-Google_Slides-yellow?logo=googleslides&logoColor=white)](https://docs.google.com/presentation/d/1YjRIxj32OXhiaPgXihWKW40aPGhIcgBFr4CPkJLY19Q/edit?usp=sharing) |
| 🤖 Diffusion Policy – Columbia University | [![Website](https://img.shields.io/badge/Open-Project-blue?logo=googlechrome)](https://diffusion-policy.cs.columbia.edu/) |
| 🧠 Imitating Human Behavior with Diffusion Models (2023) | [![arXiv](https://img.shields.io/badge/arXiv-2301.10677-b31b1b?logo=arxiv)](https://arxiv.org/abs/2301.10677) |
| 📐 Geometry of Diffusion Models for Robotics – Sander Dieleman | [![Blog](https://img.shields.io/badge/Read-Blog-orange?logo=readthedocs)](https://sander.ai/2023/08/28/geometry.html) |
| 🧩 Ensemble of Costs for Diffusion Planning | [![Website](https://img.shields.io/badge/Open-Project-blue?logo=googlechrome)](https://ensemble-of-costs-diffusion.github.io/) |
| 💎 DIAMOND – Diffusion Models for Diverse Robot Behavior | [![Website](https://img.shields.io/badge/Open-Project-blue?logo=googlechrome)](https://diamond-wm.github.io/) |
| 🚗 Imagine2Drive – Open Vocabulary Driving Skills | [![Website](https://img.shields.io/badge/Open-Project-blue?logo=googlechrome)](https://anantagrg.github.io/Imagine-2-Drive.github.io/) |
| 🧞 GENIE (Diffusion + LLMs) – Google DeepMind | [![Website](https://img.shields.io/badge/Open-Project-blue?logo=googlechrome)](https://sites.google.com/view/genie-2024/home) |
| 🌌 DreamGen – Scene-Level Robot Imagination (NVIDIA) | [![Website](https://img.shields.io/badge/Open-Project-blue?logo=googlechrome)](https://research.nvidia.com/labs/gear/dreamgen/) |
| 🌀 Diffusion Forcing – Diffusion Models for Human Motion Imitation | [![Website](https://img.shields.io/badge/Open-Project-blue?logo=googlechrome)](https://boyuan.space/diffusion-forcing/) |
| 🔄 Flow Matching – Machine Learning Group, University of Cambridge | [![Blog](https://img.shields.io/badge/Read-Blog-orange?logo=readthedocs)](https://mlg.eng.cam.ac.uk/blog/2024/01/20/flow-matching.html) |



---