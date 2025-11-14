# Reinforcement Learning Assignment 3

| Name | Student Number | Course | Course Code |
|------|----------------|--------|-------------|
| Christo Pananjickal Baby | 8989796 | Reinforcement Learning Programming | CSCN 8020 |

## Overview
In this assignment, we implement a **Deep Q-Network (DQN)** agent to play **Pong** using the Atari Learning Environment. The goal is to train the agent to learn a policy that maximizes cumulative rewards by exploring the game environment and estimating Q-values for each action. Experiments are conducted to observe how **mini-batch size** and **target network update rate** affect training stability and early learning performance.

## Project Structure
- **lib/**: Contains all Python code for the DQN implementation, training scripts, and utility functions.
- **Plots/**: Contains plots of episode rewards and Avg5 metrics (optional, if saved during training).
- **README.md**: Quick intro to the assignment.  
- **documents**: This folder contains the word and PDF document for the assignment.  

## Steps to Run
1. Clone the repository:
```bash
git clone https://github.com/Christo-Conestoga-AIML/RL-Assignment-3.git
```
2. Navigate to the project folder
```bash
cd RL-Assignment-3
```
3. Install required packages:
```bash
pip install -r requirements.txt
```
4. Run the training script:
```bash
python lib/assignment_3.ipynb
```
5. Training logs and reward plots will be displayed and in the shell output.

## Notes
- Input frames are preprocessed and stacked as 4 consecutive images for the CNN.

- Metrics tracked include Score per Episode and Average cumulative reward of the last 5 episodes (Avg5).

- Best configuration observed: Batch Size = 8, Target Network Update = every 3 episodes.