# Lecture 22: Reinforcement Learning
**Instructors:** Vishal, Tejas    
**Date:** June 13, 2025 

## 📖 Topics Covered:

- **1. Why Reinforcement Learning?**
  - Why is it hard to generate data for robots with frequently changing morphologies?
  - Why are traditional approaches (e.g., explicit physics models, controllers) inefficient for skill learning?
  - How does RL (and supervised learning) help bridge this gap?
  - What is an example where RL enabled fast adaptation (e.g., quadrupeds using rapid motor adaptation)?

- **2. RL Notation and Terminology**
  - What are stochastic processes and the Markovian property?
  - What is a Markov Decision Process (MDP), and how is it defined?

- **3. Anatomy of the Reinforcement Learning Pipeline**
  - How do we collect samples from the environment using the current policy?
  - What does model fitting or sample evaluation involve?
  - How is the policy improved based on evaluation?
  - How do modern simulators and sim-to-real transfer help overcome sample collection bottlenecks?

- **4. Policy Gradient Methods**

  **4.1 Goal of RL**
  - What is the objective function \( J(\theta) \) in RL?
  - How does the formulation differ in finite vs. infinite horizon settings?
  - Why is the goal to maximize expected return?

  **4.2 Policy Gradient**
  - How do we compute the gradient of the objective function?
  - What is the REINFORCE trick and algorithm?

- **5. Reducing Variance in REINFORCE**
  - Why does REINFORCE have high variance despite being unbiased?
  - How does the reward-to-go trick exploit causality to reduce variance?
  - What are baseline methods for variance reduction?
  - How do we choose an optimal baseline to minimize variance?
  - What are actor-critic methods, and how do they combine value estimation with policy updates?

- **6. Value-Based Methods**
  - Value function and Q-function
  - What are SARSA and Q-learning?
  - How does Deep Q-Learning extend traditional Q-learning?


## 📄 Assignment

- 🧠 **Policy Gradient & Actor-Critic Walkthrough:**  
   Open the following Colab notebook to implement and experiment with Policy Gradient methods from scratch:  
   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1TWPHz3udlKqsdSyMvTiZG9Y5P7VrY3gH?usp=sharing)

   This walkthrough is designed to help you implement a working **Policy Gradient agent** using PyTorch on environments like *CartPole*.

   ---

   **📚 What You'll Learn**
   - Core ideas behind Policy Gradient algorithms
   - How to implement and train a neural network policy
   - How to collect rollouts and compute returns
   - Policy updates using gradient ascent
   - (Optional) Baseline methods & Generalized Advantage Estimation (GAE)

   **🛠 Prerequisites**
   - Python + PyTorch basics
   - Key RL concepts: Policy, Reward, Return, Advantage, Value Function

   **🗂 Notebook Structure**
   - **Environment Setup**: Logging and configuration
   - **Policy Network**: Implementation and sampling
   - **Training Loop**: Computing returns and updating the policy
   - **Variance Reduction (Optional)**: Baselines, GAE for stability

   **👨‍🏫 Tips for Students**
   - Run cells in order — don’t skip!
   - Print out observations, actions, rewards to debug.
   - Try different hyperparameters and Gym environments.
   - Use TensorBoard or video logs to visualize progress.

   > 📘 Inspired by [CS285: Deep RL (Berkeley)](https://rail.eecs.berkeley.edu/deeprlcourse/)
   
   _Courtesy: Tejas_

📢 Do post doubts on the `#module-7-robot-learning` Slack channel!

## 🔗 Resources

| 📚 Topic | 🔗 Link |
|----------|---------|
|Lecture Slides -- Reinforcement Learning| See Lectures 4-7 from RAIL Course (linked below) |
| 🎓 Deep Reinforcement Learning – Sergey Levine (RAIL, Berkeley) | [![Website](https://img.shields.io/badge/Open-Course-blue?logo=googleclassroom)](https://rail.eecs.berkeley.edu/deeprlcourse/) |
| 🧠 Policy Gradient Algorithms – Lilian Weng | [![Blog](https://img.shields.io/badge/Read-Blog-orange?logo=readthedocs)](https://lilianweng.github.io/posts/2018-04-08-policy-gradient/) |
| ⚙️ PPO Implementation Details – ICLR Blog Track | [![Blog](https://img.shields.io/badge/Read-PPO_Insights-orange?logo=readthedocs)](https://iclr-blog-track.github.io/2022/03/25/ppo-implementation-details/) |
| 📘 Mathematical Foundations of RL – Shiyu Zhao (Westlake University) | [![GitHub](https://img.shields.io/badge/View-on_GitHub-181717?logo=github)](https://github.com/MathFoundationRL/Book-Mathematical-Foundation-of-Reinforcement-Learning) |
| ⚡ RL Quickstart Guide – Joseph Suarez (Pufferlib Creator) | [![X/Twitter](https://img.shields.io/badge/View-Quickstart_Guide-1DA1F2?logo=x)](https://x.com/jsuarez5341/status/1854855861295849793) |
| 📦 Stable Baselines3 – RL Library (DLR-RM) | [![GitHub](https://img.shields.io/badge/View-Stable--Baselines3-181717?logo=github)](https://github.com/DLR-RM/stable-baselines3) |
| 🧼 CleanRL – Minimal RL Implementations | [![GitHub](https://img.shields.io/badge/View-CleanRL-181717?logo=github)](https://github.com/vwxyzjn/cleanrl) |
| 🐉 Decisions & Dragons – FAQs About RL | [![Website](https://img.shields.io/badge/Explore-Decisions_&_Dragons-blueviolet?logo=readthedocs)](https://www.decisionsanddragons.com/) |

---