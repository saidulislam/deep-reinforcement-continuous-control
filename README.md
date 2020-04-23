## Deep Reinforcement Learning Nanodegree (Udacity)
## Project 2: Continuous Control

<img src="images/reacher.png" align="top-left" alt="" title="Plot" />

For this project, I worked with the [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment and trained it using a Reinforcement Learning (RL) model  for continuous controls.

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of the agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

## Distributed Training
For this project, we were given two separate versions of the Unity environment:

- The first version contains a single agent.
- The second version contains 20 identical agents, each with its own copy of the environment.
The second version is useful for algorithms like PPO, A3C, and D4PG that use multiple (non-interacting, parallel) copies of the same agent to distribute the task of gathering experience.

I couldn't get the second version to work and thus, for the project submission, I stuck to the single agent (first version).

## Running the Project
I am using Jupyter Notebook for the project. Running all the cells from top to bottom in the notebook will install the necessary packages and train our agent.

Important project files:

- Continuous_Control.ipynb - Jupyter notebook project file.
- model.py - Actor and Critic models
- ddpg_agent.py - DDPG Agent class
- checkpoint_actor.pth - Actor trained model
- checkpoint_critic.pth - Critic trained model
