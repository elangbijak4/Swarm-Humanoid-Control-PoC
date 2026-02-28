# Swarm-Based Humanoid Coordination (Proof of Concept)

This repository contains the reproducible Python implementation of the distributed swarm-based humanoid coordination architecture presented in:

**"Swarm-Based Coordination Architecture for Humanoid Robots: A Distributed Multi-Agent Framework with Secure Rule Evolution"**

## Overview

This project demonstrates how stable global behavior can emerge from purely local swarm interaction rules without centralized trajectory optimization or rigid-body dynamic modeling.

Each joint is modeled as an autonomous 2D agent governed by:

- Alignment interaction
- Cohesion interaction
- Stability-seeking behavior

A lightweight secure rule evolution mechanism is also implemented using SHA-256 hashing and distributed consensus voting.

## Implemented Components

- Distributed 2D joint-agent simulation
- Swarm-based decentralized update rule
- Centralized baseline controller
- Disturbance injection protocol
- Stability Index computation
- Recovery time measurement
- Secure rule evolution (hash + 70% consensus threshold)
- Scalability evaluation (N = 10, 20, 50, 100)

## Reproducibility

All numerical results reported in the paper (stability index, recovery time, scalability behavior, and malicious rule rejection) can be reproduced by executing the provided notebook.

Random seed is fixed for deterministic results.

## How to Run

### Option 1 — Google Colab

1. Open the notebook in Google Colab.
2. Run all cells sequentially.
3. Tables and plots will be generated automatically.

### Option 2 — Local Execution

Requirements:
- Python 3.9+
- numpy
- matplotlib

Install dependencies:

```bash
pip install numpy matplotlib
