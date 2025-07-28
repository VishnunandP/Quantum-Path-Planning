# Quantum-Inspired Reusable Path Planning System

This project implements a dynamic path planning system that simulates reusable trajectory discovery under adversarial environments. Inspired by quantum sampling principles, the system generates multiple stochastic paths, evaluates them using entropy-based heuristics, and filters for reusable high-fidelity candidates. A dynamic grid world introduces random obstacle shifts over time, enabling benchmarking against conventional A* search in terms of compute efficiency and path robustness.

## Features
- Quantum-inspired stochastic path sampling with entropy-aware filtering
- Custom action functional combining path length, curvature, and obstacle risk
- Dynamic environment simulation with evolving obstacles
- A* benchmark integration for runtime and path optimality comparison
- Detailed performance visualization: compute time, entropy distribution, reuse decay

## Technologies
Python, NumPy, Matplotlib, Heapq, Random

## Project Structure
- `GridWorld`: Modular environment with obstacle generation and validation
- `a_star`: Deterministic baseline pathfinding algorithm
- `sample_paths`: Probabilistic trajectory generator with tunable entropy threshold
- `simulate_dynamic_environment`: Temporal simulation to test path reuse
- `visualization`: Plots comparing cumulative compute time, reuse rate, entropy, and action cost

## Usage
All scripts are executable in Jupyter or standard Python environments. Recommended flow:
1. Generate environment and obstacles
2. Run A* baseline
3. Sample quantum-inspired paths
4. Filter by entropy
5. Simulate dynamic environment and evaluate reuse
6. Visualize results

## Results Summary
- Demonstrated significant runtime savings using precomputed paths
- Quantified tradeoffs between compute efficiency and trajectory quality
- Built fully automated simulation with interpretable metrics and visuals



