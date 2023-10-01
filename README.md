# ReacherProject

## Project Details
The project consists of solving the Reacher environment which is a double-jointed arm that moves to target locations.
-	State Space: consists of 33 continuous variables corresponding to the position, rotation, velocity, and angular velocities of the arm
-	Action space: consists of 4 continuous variables between -1 and 1
-	Reward: The agent gets a reward of +0.1 each time his hand is the goal location
The environment has 2 versions, one composed of a single agent, and the other of 20 agents. Although numerous attempts were made to solve the environment compose of a single agent, I found it easier and faster to solve the environment composed of 20 agents.
The environment is considered solved when the average score over the 20 agents is higher than 30 on average for 100 episodes.

## Repository Structure
This repository is composed of:
- Actor weights: actor_checkpoint.pth
- Critic weights: critic_checkpoint.pth
- Project report: Report.pdf
- Project main notebook: Continuous_Control.ipynb

## Getting Started
In the Continuous_Control.ipynb:
- Install the dependencies by running the first cell of the notebook in Start the Environment section.
- Start the environment by running the second cell.

## Instructions
The Continuous_Control.ipynb is composed of multiple sections:
1. Start the Environment: to start the environment
2. Examine the State and Action Spaces: to examine the State and Action spaces
3. Utilities function to retrieve the state, reward and done when executing an action in the environment
4. Agent dependencies and hyperparameters to finetune when training
5. Critic and Actor models architectures
6. Replay buffer for past experiences: to store experiences and sample training batches
7. Deep Deterministic Policy Gradient agent model: agent class
8. Agent training function: agent training function definition
9. Agent training results: to run the training function and retrieve the agent scores
10. Agent training scores plot: plot the agent scores
To run the training function, you can execute the notebook cells in order until section 9 included.
To finetune the agent hyperparameters, you can change section 4 values.

