# Deep Q-Learning for Lunar Landing

This project implements a Deep Q-Network (DQN) agent to solve the Lunar Lander environment from the OpenAI Gym.

## Project Overview

The goal of this project is to train an AI agent to land a lunar lander safely on the moon's surface using Deep Reinforcement Learning. The DQN agent learns to map states to actions by maximizing its cumulative reward over time.

## Algorithm and Approach

- **Deep Q-Learning:** The project uses the DQN algorithm, a model-free, off-policy reinforcement learning algorithm that utilizes a neural network to approximate the Q-function.
- **Experience Replay:** The agent stores its experiences in a replay buffer and samples random batches of experiences to learn from, improving the stability and efficiency of training.
- **Target Network:** A separate target network is used to stabilize training by providing a consistent target for the Q-function updates.
- **Epsilon-Greedy Exploration:** The agent balances exploration and exploitation using an epsilon-greedy strategy, gradually decreasing the exploration rate (epsilon) over time.

## Usage

To run the project, simply execute the cells in the provided Jupyter Notebook in sequential order. The notebook is divided into three parts:

1. **Building the AI:** Defines the architecture of the neural network used by the DQN agent.
2. **Training the AI:** Sets up the environment, initializes hyperparameters, implements experience replay and the DQN class, and trains the agent.
3. **Visualizing the results:** Generates a video of the trained agent interacting with the environment.

## Hyperparameters

The following hyperparameters are used in the project:

- Learning rate: 5e-4
- Minibatch size: 100
- Discount factor: 0.99
- Replay buffer size: 1e5
- Interpolation parameter: 1e-3
- Number of episodes: 2000
- Maximum number of timesteps per episode: 1000
- Epsilon starting value: 1.0
- Epsilon ending value: 0.01
- Epsilon decay value: 0.995

## Results

The trained DQN agent achieves an average score of 200 or higher on the Lunar Lander environment, indicating successful completion of the task.
