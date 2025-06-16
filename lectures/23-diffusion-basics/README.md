# Lecture 23: Diffusion Models Basics
**Instructor:** Anant Garg    
**Date:** June 14, 2025

## Topics Covered:

- Noise, Gaussians + Setup
- Autoencoders, VAE, Reparameterization Trick
- The Forward Process: Adding Noise Step-by-Step  
- The Reverse Process: Learning to Denoise  
- DDPM: Predicting Noise to Reconstruct Data  
- Guidance: Making Diffusion Outputs Useful  
  - Classifier-Based
  - Classifier-Free
- Score Matching
- Latent Diffusion

## 📄 Assignment

- 🎨 **Diffusion Models – DDPM & Stable Diffusion Walkthroughs:**  
   Clone and run through the following two PyTorch implementations to understand the fundamentals of diffusion models:

   - 📦 **DDPM (Denoising Diffusion Probabilistic Models):**  
     [explainingai-code/DDPM-PyTorch](https://github.com/explainingai-code/DDPM-Pytorch)

     This repo walks through the original DDPM algorithm in PyTorch. Run the code, visualize the forward and reverse diffusion process, and study how noise schedules influence generation.

     🔁 **Extension Task – Implement DDIM:**  
     Read [DDIM paper (arXiv:2010.02502)](https://arxiv.org/abs/2010.02502) and extend the code to include deterministic sampling via DDIM.  
     Suggested steps:
     - Modify the sampling loop to use DDIM's non-Markovian formulation
     - Add support for fewer inference steps (fast sampling)
     - Compare image quality vs sampling speed with DDPM

   - 🎨 **Stable Diffusion (from scratch):**  
     [explainingai-code/StableDiffusion-PyTorch](https://github.com/explainingai-code/StableDiffusion-PyTorch)

     This repo walks through a simplified but faithful re-implementation of Stable Diffusion.  
     Explore how text prompts are encoded, how the UNet denoiser operates, and how the latent diffusion process differs from vanilla DDPM.

💡 Feel free to experiment with prompts, noise schedules, and decoder resolutions! Post all your findings, doubts on the `#module-7-robot-learning` Slack channel.

## 🔗 Resources

| 📚 Topic | 🔗 Link |
|----------|--------|
| 📑 Lecture Slides – Diffusion Basics | [![PDF](https://img.shields.io/badge/Open-Slides-red?logo=adobeacrobatreader&logoColor=white)](./lec-23-diffusion-basics.pdf) |
| 🧠 From Autoencoder to Beta-VAE – Lilian Weng | [![Blog](https://img.shields.io/badge/Read-Blog-orange?logo=readthedocs)](https://lilianweng.github.io/posts/2018-08-12-vae/) |
| 🌫️ What Are Diffusion Models? – Lilian Weng | [![Blog](https://img.shields.io/badge/Read-Blog-orange?logo=readthedocs)](https://lilianweng.github.io/posts/2021-07-11-diffusion-models/) |
| 📄 DDPM – Denoising Diffusion Probabilistic Models (Ho et al.) | [![PDF](https://img.shields.io/badge/Open-Paper-blue?logo=readthedocs)](https://hojonathanho.github.io/diffusion/) |
| 🧬 Latent Diffusion Models – High-Res Image Synthesis | [![arXiv](https://img.shields.io/badge/arXiv-2112.10752-b31b1b?logo=arxiv)](https://arxiv.org/pdf/2112.10752) |
| 🎥 Explaining Diffusion – YouTube Playlist | [![YouTube](https://img.shields.io/badge/Watch-Playlist-red?logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PL8VDJoEXIjpo2S7X-1YKZnbHyLGyESDCe) |
| 🧪 Stable Diffusion (from scratch) – PyTorch Codebase | [![GitHub](https://img.shields.io/badge/View-Code-181717?logo=github)](https://github.com/explainingai-code/StableDiffusion-PyTorch) |
| 🌊 Introduction to Flow Matching & Diffusion Models – MIT 6.S184 (Generative AI with SDEs) | [![Website](https://img.shields.io/badge/Open-Course-blue?logo=mit&logoColor=white)](https://diffusion.csail.mit.edu/) |
| 🎥 Diffusion Models – Paper Explanation & Math | [![YouTube](https://img.shields.io/badge/Watch-Video-red?logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=HoKDTa5jHvg) |
| 🎓 CS 198-126: Lecture 12 – Diffusion Models (ML@Berkeley) | [![YouTube](https://img.shields.io/badge/Watch-Lecture-red?logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=687zEGODmHA&t=23s) |


---