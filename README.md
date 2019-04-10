# RL_continuous_control
## Introduction
This repo is an implement of Unity's Reacher with [DeepDPG](https://arxiv.org/abs/1509.02971) alogrithm

The reacher environment is shown below. a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal the agent(s) is to maintain its position at the target location for as many time steps as possible.
<p align="center">
<img src="https://s3.amazonaws.com/video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif">
</p>
## Project Details
Here are the environment details from Unity. The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints.
```
    Vector Observation space size (per agent): 33
    Number of stacked Vector Observation: 1
    Vector Action space type: continuous
    Vector Action space size (per agent): 4
```
File model.py contains the network (Actor and Critic) for DeepDPG and ddpg_agent.py contains policy for agent to make action. Run Continuous_Control.ipynb to see the details.

## Depedency
- python 3.6
- [ml-agents](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) from Unity
- Numpy
- pytorch(0.4.0)


