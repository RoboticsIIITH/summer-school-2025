# Lecture 09: Deep Learning - II

**Instructor:** Gaurav  
**Date:** May 27, 2025

---

## 📖 Overview

In this lecture, we explore the critical role of **activation functions** in introducing non-linearity to neural networks, enabling them to model complex relationships. We cover popular activation functions such as **Sigmoid**, **Tanh**, **ReLU**, **Leaky ReLU**, **ELU**, and **Swish**, discussing their characteristics, advantages, and pitfalls, including issues like vanishing and exploding gradients.

We then delve into **regularization techniques** to prevent overfitting and improve generalization. We examine **L1 (Lasso)** and **L2 (Ridge)** regularization, highlighting their effects on weight shrinkage and sparsity. Additionally, we discuss **Dropout**, a stochastic method that randomly deactivates neurons during training, and its impact on network robustness.

Finally, we introduce **Batch Normalization** and **Layer Normalization** as methods to accelerate training, reduce internal covariate shift, and stabilize learning. We compare their mechanisms, use cases, and implementation details.

---

## 📄 Assignment

- **Exercise Notebooks:**
  - [activation-function-basics.ipynb](activation-function-basics.ipynb)
  - [batch-normalization.ipynb](batch-normalization.ipynb)

Please submit any questions or discussion points on the **`#module-3-deep-learning`** Slack channel.

---

## 🔗 Resources

| Topic                              | Link                                                                                     |
|------------------------------------|------------------------------------------------------------------------------------------|
| Lecture Slides - Deep Learning - Activation Funtions, Regularization                     | [lec-09-dl-training.pdf](./lec-09-dl-training.pdf)                     |

---

## 🧠 Notes

- **Activation Functions**  
  - *Sigmoid*: Outputs in (0,1), smooth gradients, but suffers from vanishing gradients in deep nets.  
  - *Tanh*: Zero-centered output in (–1,1), better convergence than Sigmoid but still susceptible to vanishing gradients.  
  - *ReLU*: $f(x)=\max(0,x)$, sparse activation, mitigates vanishing gradients but can “die” for negative inputs.  
  - *Leaky ReLU*: $f(x)=\max(\alpha x,x)$, allows small gradient for $x<0$, alleviates “dying ReLU” problem.  
  - *ELU, Swish*: Smooth alternatives that can outperform ReLU in certain tasks.

- **Regularization**  
  - *L1 Regularization*: Adds $\lambda \lVert w \rVert_1$ penalty, encourages weight sparsity—useful for feature selection.  
  - *L2 Regularization*: Adds $\tfrac{\lambda}{2} \lVert w \rVert_2^2$ penalty, prevents large weights via weight decay and yields smoother solutions.  
  - *Dropout*: Randomly zeroes activations with probability $p$ during training, reducing neuron co-adaptation and effectively ensembling sub-networks.

- **Normalization Techniques**  
  - *Batch Normalization*: Normalizes layer inputs per mini-batch to zero mean and unit variance, followed by learnable scale and shift. Reduces internal covariate shift and enables higher learning rates.  
  - *Layer Normalization*: Normalizes across features for each sample independently, beneficial for RNNs and scenarios with small batch sizes.
