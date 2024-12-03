# Space-Time: A Reinforcement Learning Adventure

Welcome to Space-Time, a reinforcement learning project where intelligent agents navigate a grid-world environment filled with static and dynamic obstacles to reach a target goal. The project benchmarks different RL algorithms to evaluate their performance in this complex scenario.

# Project Overview
In Space-Time, agents are tasked with controlling a spaceship navigating a hazardous space grid. Obstacles include asteroids (static) and alien crafts (dynamic). The goal is to reach the space station safely, avoiding collisions and maximizing rewards.

The project compares the performance of four popular deep reinforcement learning algorithms:

1) Deep Q-Learning (DQN) 
2) Double DQN (DDQN) 
3) Dueling DQN
4) Prioritized Experience Replay (PER)

After evaluation, only the algorithms achieving positive average rewards are retained for further exploration.

# Key Features

A customizable grid-world environment with dynamic visuals using Pygame.
Static (asteroids) and moving (alien crafts) obstacles for enhanced complexity.
Algorithm comparison based on average rewards.
Real-time visualization of training and agent decisions.

## Algorithm Results

| Algorithm     | Average Reward |
|---------------|----------------|
| DQN           | 23.17          |
| Double DQN    | -17.35         |
| Dueling DQN   | 23.41          |
| PER           | -24.95         |


Only DQN and Dueling DQN proceed for further testing due to their positive rewards.

# Structure
## Project Structure

- Space-Time/
  - `assets/` - Visual assets for the game
  - `Final.ipynb` - Jupyter Notebook for training and visualization
  - `space_mission_env.py` - Environment implementation
  - `dqn_agent.py` - RL agent code
  - `README.md` - Project documentation
  - `requirements.txt` - Dependencies


# Setup Instructions
Prerequisites
Python 3.7+
Pygame for visualization
PyTorch for implementing neural networks


# Installation

1) Clone the repository:

   git clone https://github.com/your-username/space-time.git
   
2) Install dependencies:

   pip install -r requirements.txt


# Usage
Training the Agent
1) Run the environment and agent training:
      python Final.ipynb
2) Select an RL algorithm from the provided options (DQN, DDQN, Dueling DQN, or PER).


# Visualizing the Game
The pygame window will render the grid, spaceship, obstacles, and goal dynamically during training.

# Results and Insights
This project demonstrates how reinforcement learning algorithms perform under varying complexity. Key findings:

 1) DQN and Dueling DQN effectively learn to navigate the grid and achieve positive rewards.
 2) DDQN and PER fail to generalize, leading to negative average rewards.
    
Further optimizations and exploration are possible by modifying hyperparameters or grid configurations.

# Contributing
Contributions are welcome! Please fork the repository and submit a pull request. For significant changes, open an issue to discuss your proposed modifications.

