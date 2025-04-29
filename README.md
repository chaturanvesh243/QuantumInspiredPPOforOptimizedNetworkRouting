# QuantumInspiredPPOforOptimizedNetworkRouting
Quantum-Inspired Reinforcement Learning for Network Routing Optimization
This project implements a quantum-inspired reinforcement learning approach for adaptive network routing optimization. By integrating quantum computing concepts-such as superposition, interference, and measurement-into classical reinforcement learning (PPO), the system achieves superior performance in dynamic network environments compared to traditional and standard RL-based routing methods.

Features
Quantum-Inspired Neural Networks: Complex-valued layers simulate quantum effects for richer state representation and enhanced exploration.

Enhanced PPO Algorithm: Proximal Policy Optimization is extended with quantum-inspired components.

Realistic Network Simulation: Supports random, scale-free, and small-world topologies with dynamic traffic, failures, and congestion.

Multi-Objective Optimization: Balances packet delivery, latency, throughput, and resource utilization.

Comprehensive Evaluation: Includes baseline algorithms (OSPF, ECMP, Q-Routing, DQN, PPO) for fair comparison.

Project Structure
text
.
├── README.md
├── requirements.txt
├── main.py
├── network/
│   ├── topology.py
│   ├── traffic.py
│   └── environment.py
├── agents/
│   ├── ppo.py
│   ├── quantum_ppo.py
│   └── baselines.py
├── quantum/
│   ├── encoder.py
│   ├── layers.py
│   └── measurement.py
├── evaluation/
│   ├── metrics.py
│   └── analysis.py
└── experiments/
    └── configs/
Installation
Clone the repository:

bash
git clone https://github.com/chaturanvesh243/QuantumInspiredPPOforOptimizedNetworkRouting.git
cd QuantumInspiredPPOforOptimizedNetworkRouting
Install dependencies:

bash
pip install -r requirements.txt
Main dependencies include: numpy, torch, networkx, matplotlib, gym, tensorboard.

Usage
Training
Train the quantum-inspired PPO agent on a random topology:

bash
python main.py --agent quantum_ppo --topology random --episodes 1000
Train a baseline agent (e.g., PPO):

bash
python main.py --agent ppo --topology random --episodes 1000
Evaluation
Evaluate trained agents and compare metrics:

bash
python main.py --evaluate --agent quantum_ppo
Visualization
To visualize training progress and results:

bash
tensorboard --logdir logs/
Configuration
Network Topology: Choose from random, scale_free, or small_world.

Training Parameters: Set via command-line or config files (episodes, batch size, learning rate, etc.).

Quantum Parameters: Adjustable quantum dimension, interference paths, and phase settings.

Results
Quantum-inspired PPO outperforms classical baselines:

+4.3% packet delivery ratio

-12.7% end-to-end delay

+6.2% throughput

30-33% faster convergence

See the results section for detailed plots and analysis.

References
Proximal Policy Optimization Algorithms

Quantum Computation and Quantum Information (Nielsen & Chuang, 2010)

Quantum machine learning (Nature, 2017)

License
This project is licensed under the MIT License.

Contact
For questions or collaboration, please contact chaturanvesh.kethiri@gmail.com

This project demonstrates how quantum-inspired algorithms can enhance classical reinforcement learning for complex, real-world optimization problems like network routing.
