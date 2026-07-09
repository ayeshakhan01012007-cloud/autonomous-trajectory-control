# 🚁 Autonomous Trajectory Tracking with Wind Disturbance Handling

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Control Systems](https://img.shields.io/badge/Control-PID%20%26%20PD-green)
![Simulation](https://img.shields.io/badge/Simulation-Matplotlib-orange)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-red)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📖 Overview

This project demonstrates the implementation of classical feedback control algorithms for autonomous vehicle trajectory tracking under external disturbances.

Two autonomous systems are simulated:

* 🚤 **Surface Boat Guidance System** – Navigates through water currents using a tuned **PD controller**.
* 🚁 **Drone Figure-Eight Tracking System** – Tracks a complex figure-eight trajectory while compensating for constant wind disturbances using a **PID controller**.

The objective is to maintain accurate path tracking despite environmental forces that continuously push the vehicle away from its desired trajectory.

---

## 🎯 Objectives

* Simulate autonomous trajectory tracking.
* Generate complex reference trajectories.
* Model wind and water-current disturbances.
* Design and implement PD and PID controllers.
* Eliminate steady-state tracking errors.
* Visualize controller performance through animated simulations.

---

## ⚙️ System Architecture

```
Reference Trajectory
        │
        ▼
Error Calculation
        │
        ▼
  PID / PD Controller
        │
        ▼
 Vehicle Dynamics
        │
        ▼
 Wind / Water Disturbance
        │
        ▼
 Updated Position
        │
        └──────────────► Feedback Loop
```

---

## 🛠️ Technical Details

### 🚁 Drone Simulation

The drone follows a continuous figure-eight trajectory generated using the **Lemniscate of Bernoulli**.

### PID Controller

The controller consists of three components:

| Controller            | Function                                                         |
| --------------------- | ---------------------------------------------------------------- |
| **Proportional (Kp)** | Corrects current tracking error.                                 |
| **Integral (Ki)**     | Removes steady-state offset caused by constant wind disturbance. |
| **Derivative (Kd)**   | Reduces oscillations and improves system stability.              |

The addition of the **Integral (Ki)** term enables the drone to converge precisely to the desired trajectory even under persistent wind forces.

---

### 🚤 Boat Simulation

The boat simulation models navigation through cross-water currents.

A tuned **PD controller** provides:

* Fast response
* Stable navigation
* Smooth trajectory correction
* Reduced oscillation

---

## 🌪️ Disturbance Modeling

The simulations include realistic environmental disturbances:

* Constant wind force acting on the drone
* Cross-current disturbance acting on the boat

The control system continuously compensates for these disturbances through closed-loop feedback.

---

## 📂 Repository Structure

```
📁 Autonomous-Trajectory-Tracking
│
├── Advanced_drone_technology.ipynb
├── README.md
└── requirements.txt (optional)
```

---

## 🚀 Features

* Figure-eight trajectory generation
* Wind disturbance simulation
* Water-current simulation
* PD controller
* PID controller
* Closed-loop feedback control
* Real-time trajectory animation
* Clean and modular Python implementation

---

## 💻 Technologies Used

* Python 3
* NumPy
* Matplotlib
* Matplotlib Animation
* Google Colab
* Jupyter Notebook

---

## 📈 Results

The simulation demonstrates that:

* The **PD controller** provides fast and stable tracking for the boat under varying water currents.
* The **PID controller** effectively eliminates steady-state error introduced by constant wind disturbances.
* The drone accurately follows the desired figure-eight trajectory with minimal tracking error.
* Closed-loop feedback significantly improves system robustness and overall tracking performance.

---

## 🎓 Learning Outcomes

This project provides practical experience in:

* Classical Control Systems
* Feedback Control
* PD Controller Design
* PID Controller Design
* Trajectory Tracking
* Disturbance Rejection
* Autonomous Vehicle Navigation
* Scientific Computing with Python
* Data Visualization and Animation

---

## 📄 License

This project is released for educational and academic purposes.

---

**Author:** Ayesha Khan

**Course:** Aerospace Simulation Workshop

**Language:** Python

**Environment:** Google Colab / Jupyter Notebook

