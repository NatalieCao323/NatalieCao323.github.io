---
title: "VRVO: Variance-Regularized Value Optimization for Reinforcement Learning"
excerpt: "Novel RL algorithm improving generalization stability over PPO/PPG in high-variance environments, validated on OpenAI Procgen benchmark.<br/><img src='/images/vrvo-preview.png' style='max-width: 500px;'>"
collection: portfolio
---

## Project Overview

**Variance-Regularized Value Optimization (VRVO)** is a novel reinforcement learning algorithm designed to improve generalization and stability in high-variance environments. Developed during my research assistantship at the HPC-AI Lab at the National University of Singapore, VRVO addresses fundamental challenges in policy optimization by incorporating variance regularization into the value function learning process.

## Research Motivation

### The Generalization Problem in RL

Modern reinforcement learning agents often struggle to generalize from training environments to novel test scenarios. This is particularly problematic in:
- **Procedurally Generated Environments**: Where each episode presents new challenges
- **Real-World Applications**: Where deployment conditions differ from training
- **Sample-Efficient Learning**: Where limited data must support robust policies

### Existing Approaches

- **PPO (Proximal Policy Optimization)**: Industry standard, but can be unstable in high-variance settings
- **PPG (Phasic Policy Gradient)**: Improves sample efficiency but still suffers from overfitting
- **Our Contribution**: VRVO adds variance regularization to improve stability and generalization

## Technical Approach

### Core Innovation: Variance Regularization

VRVO modifies the value function learning objective to explicitly penalize high variance in value estimates:

**Standard Value Loss**: `L_V = E[(V(s) - V_target)²]`

**VRVO Value Loss**: `L_V = E[(V(s) - V_target)²] + λ·Var[V(s)]`

Where:
- `V(s)` is the learned value function
- `V_target` is the target value (e.g., TD-λ return)
- `λ` is the regularization coefficient
- `Var[V(s)]` is the variance of value estimates across similar states

### Theoretical Foundation

#### Stochastic Gradient Dynamics
We derived theoretical guarantees showing that variance regularization:
1. **Reduces Overfitting**: Smoother value functions generalize better
2. **Improves Stability**: Lower variance gradients lead to more stable training
3. **Enhances Sample Efficiency**: Better credit assignment across episodes

#### Connection to Biological Learning
The variance regularization principle mirrors biological systems that balance:
- **Stability**: Maintaining consistent behavior
- **Flexibility**: Adapting to new situations

This conceptual bridge between RL and biological systems influenced my later interest in computational biology.

## Experimental Validation

### OpenAI Procgen Benchmark

**Procgen** is a suite of 16 procedurally generated environments designed to test generalization:
- Each level is randomly generated
- Training and test distributions differ
- Requires robust, generalizable policies

### Results

| Metric | PPO | PPG | VRVO (Ours) |
|--------|-----|-----|-------------|
| **Mean Return (Train)** | 8.2 | 8.7 | 8.9 |
| **Mean Return (Test)** | 6.1 | 6.5 | **7.3** |
| **Generalization Gap** | 2.1 | 2.2 | **1.6** |
| **Training Stability (σ)** | 1.8 | 1.5 | **1.2** |

**Key Findings**:
- **19% improvement** in test performance over PPO
- **12% improvement** over PPG
- **24% reduction** in generalization gap
- **20% improvement** in training stability

### Ablation Studies

1. **Regularization Coefficient (λ)**: Optimal value around 0.01-0.05
2. **Network Architecture**: Consistent improvements across different architectures
3. **Environment Complexity**: Larger gains in more complex environments
4. **Sample Efficiency**: Comparable sample efficiency to PPG

## Implementation Details

### Algorithm Components

1. **Policy Network**: Actor network with entropy regularization
2. **Value Network**: Critic network with variance regularization
3. **Optimization**: Adam optimizer with learning rate scheduling
4. **Clipping**: PPO-style clipping for policy updates

### Hyperparameters

- Learning rate: 3e-4 (policy), 1e-3 (value)
- Variance regularization: λ = 0.03
- Discount factor: γ = 0.99
- GAE parameter: λ_GAE = 0.95
- Batch size: 2048 transitions
- Epochs per update: 3

### Computational Resources

- **Hardware**: NVIDIA A100 GPUs
- **Training Time**: ~24 hours for full Procgen suite
- **Framework**: PyTorch, Stable-Baselines3

## Connections to Biological Systems

This project revealed deep connections between RL and biological learning:

### Adaptive Systems Under Uncertainty
Both RL agents and biological cells must:
- **Balance exploration and exploitation**
- **Maintain stability while adapting**
- **Generalize from limited experience**

### High-Dimensional Stochastic Spaces
- **RL**: State-action spaces with stochastic transitions
- **Biology**: Cell state spaces with stochastic gene expression

These parallels inspired my transition to computational biology, where similar mathematical frameworks can model:
- Cell fate decisions (analogous to policy optimization)
- Developmental trajectories (analogous to RL trajectories)
- Gene regulatory networks (analogous to value functions)

## Publications & Dissemination

### Manuscripts
- **Paper**: "Improving Generalization of Reinforcement Learning via VRVO" (under review)
- **Book Chapter**: Contributing author to "The Application of AI Large Models" (ISBN: 9787111738787)

### Presentations
- HPC-AI Lab seminar series
- Internal research discussions at Stanford

## Code & Reproducibility

- **Framework**: Built on Stable-Baselines3
- **Environment**: OpenAI Procgen
- **Reproducibility**: Detailed hyperparameters and random seeds provided

## Future Directions

### Algorithmic Extensions
1. **Multi-Task Learning**: Extend to meta-RL settings
2. **Continuous Control**: Apply to robotics tasks
3. **Offline RL**: Adapt for batch learning scenarios

### Biological Applications
1. **Cell State Modeling**: RL for predicting cell fate transitions
2. **Drug Discovery**: Optimizing treatment strategies
3. **Protein Design**: Reinforcement learning for sequence optimization

---

**Duration**: April 2023 - September 2023  
**Institution**: HPC-AI Lab, National University of Singapore  
**Advisor**: Professor Yang You, Department of Computing  
**Status**: Manuscript under review; book chapter published  
**Skills**: Reinforcement Learning, PyTorch, Mathematical Optimization, Experimental Design
