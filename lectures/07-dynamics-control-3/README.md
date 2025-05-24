# Lecture 07: Dynamics and Control - III

**Instructor:** Sarthak  
**Date:** May 24, 2025

---

## 📖 Overview

### 🚗 Practical PID Tuning on a Low-Cost RC Car

This session was a live, hands-on demonstration of PID (specifically PD) control in action using an affordable, DIY-friendly RC car setup. The goal was to navigate the car to **3–4 specified Cartesian points** on the ground plane using only onboard sensing and wheel actuation.

Key challenges and insights:

- **Hardware constraints**:  
  The car used extremely low-cost motors, plastic gearboxes, and suffered from **wheel slip** and **low-precision actuation**—making it a perfect real-world control testbed.
  
- **PD (Proportional-Derivative) Control**:  
  Due to noisy motor response and unreliable integral feedback, only **PD tuning** was applied. Students observed:
  - The effect of increasing **P**: faster correction but more oscillation.
  - The role of **D**: damping and stabilization during approach to the target.

- **Control Strategy**:  
  The controller attempted to align the heading and drive straight toward each target sequentially, correcting angular error and linear error using separate PD loops.

---

## 📄 Assignment

## 🚀 Simulate a 2D Self-Landing Rocket

You are tasked with simulating a **2D rocket landing scenario** using Python. Your rocket begins at a known altitude and orientation and must use a **PID or LQR-based controller** to vector its thrust and land softly at a target point with minimal velocity and upright posture.

You are encouraged to use a simulation environment like **Farama Gymnasium**, or any other (e.g., pygame based simulators, custom NumPy integration). The control logic must be implemented **from scratch** using PID or LQR.

---

### Task Breakdown

#### ✅ Objectives:
- Control **horizontal and vertical position** (x, z).
- Stabilize **pitch** (θ).
- Land smoothly and upright at a fixed ground location.

#### 🔧 Rocket Dynamics:
- **2D rigid body**:
  - State: position (x, z), velocity (vx, vz), pitch θ, angular velocity ω.
  - Controls: **thrust magnitude** and **thrust angle** (relative to body).
- Include gravity and torque due to thrust offset from center of mass.

#### 💡 Steps:
1. **Set Up Rocket Dynamics**
   - Use time-stepped integration (Euler or better).
   - Simulate body forces and motion.

2. **Implement PID or LQR Controller**
   - Control thrust direction and pitch for stable descent.
   - Tune gains for minimal overshoot and soft landing.

3. **Visualize the Landing**
   - Use simulation environment visuals (or `matplotlib` for debugging).
   - Optional: plot trajectories, thrust vectors, pitch over time.

---

### 🧠 Controller Requirements

- Your controller must output:
  - Thrust **magnitude**
  - Thrust **angle**
- You **must write your own controller code** (no built-in PID libraries).
- Keep your implementation modular and easy to tune.

---

### 🧪 Evaluation Criteria

| Criteria                 | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| Stability                | Rocket should land softly without tumbling.                                |
| Orientation              | Final pitch angle near zero (upright).                                     |
| Trajectory               | Realistic motion with controlled descent.                                  |
| Code Quality             | Clear structure, reusable functions, good comments.                        |
| Visualization (Bonus)    | Animations or trajectory plots help illustrate your approach.              |

---

### 🌐 Resources

- 🔗 [Gymnasium Documentation](https://gymnasium.farama.org/)
- 🔗 [2D Lunar Lander (OpenAI Gym)](https://github.com/openai/gym/blob/master/gym/envs/box2d/lunar_lander.py)

---

📢 Share your progress, visuals, and questions in the **`#module-2-dynamics-control`** Slack channel!

🎥 You’re encouraged to include a **GIF or short animation** of your simulation in your submission.

---

## 🔗 Resources

| Topic                                  | Link                                                                                                       |
|---------------------------------------|------------------------------------------------------------------------------------------------------------|
| Brian Douglas's Control Theory Series | [YouTube Playlist](https://youtube.com/playlist?list=PLUMWjy5jgHK3j74Z5Tq6Tso1fSfVWZC8L&feature=shared)     |
| Control Bootcamp by Steve Brunton     | [YouTube Playlist](https://youtube.com/playlist?list=PLMrJAkhIeNNR20Mz-VpzgfQs5zrYi085m&si=a-w7uEgV6jlZdMlL) |

---
