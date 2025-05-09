# AIoT-DQN Based Offloading System

A priority-aware task allocation framework for vehicular edge computing, powered by a Double Deep Q-Network (DQN) enhanced with AIoT-inspired components. This implementation simulates a fleet of edge servers handling high- and low-priority vehicular tasks, learns an offloading policy via reinforcement learning, and evaluates performance in terms of task latency.

---

## Table of Contents

- [Features](#features)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Installation](#installation)  
- [Usage](#usage)  
  - [Training & Evaluation](#training--evaluation)  
- [Code Structure](#code-structure)  
- [Results](#results)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Features

- **Priority-Aware Scheduling**  
  Two-level priority queues (“high” vs. “low”) per server, with distinct weights in the reward function.  
- **Double DQN**  
  Separate policy and target networks stabilize training.  
- **AIoT Enhancements**  
  - Weighted loss for priority sampling  
  - Enhanced state representation including queue lengths, server capabilities, and simulated channel gain  
- **Simulation API**  
  Fully parameterizable task generator and server farm setup.

---

## Getting Started

### Prerequisites

- Python 3.8+  
- GPU recommended (CUDA) for faster training  

Required Python packages:

```bash
torch>=1.12.0
numpy
