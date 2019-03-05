[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/43851646-d899bf20-9b00-11e8-858c-29b5c2c94ccc.png "Crawler"


# Project 2: Continuous Control

### Introduction
This is my submission for Udacity project Continuous control. Following is the description of project:

For this project, you will work with the [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment.

![Trained Agent][image1]

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

### Solving the Environment

Note that your project submission need only solve one of the two versions of the environment. 

#### Option 1: Solve the First Version

The task is episodic, and in order to solve the environment,  your agent must get an average score of +30 over 100 consecutive episodes.

#### Option 2: Solve the Second Version

The barrier for solving the second version of the environment is slightly different, to take into account the presence of many agents.  In particular, your agents must get an average score of +30 (over 100 consecutive episodes, and over all agents).  Specifically,
- After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent.  This yields 20 (potentially different) scores.  We then take the average of these 20 scores. 
- This yields an **average score** for each episode (where the average is over all 20 agents).

The environment is considered solved, when the average (over 100 episodes) of those average scores is at least +30. 

### Getting Started

- Clone the repository using the following command:

`git clone --recurse-submodules https://github.com/sumitpai/Udacity-ContinuousControl.git`

**It is very important that you add the `--recurse-submodules` flag because rllib is an embedded sub repository. It will not be downloaded correctly without this flag.**

- Download python 3.6 and Pytorch 1.0.

- Install the unity environment as described here: [Getting Started section](https://github.com/udacity/deep-reinforcement-learning/tree/master/p2_continuous-control/README.md) (The Unity ML-agant environment is already configured by Udacity)

- The current repo has the environment for MAC. If you are using any other operating system download the corresponding build. If so, the code needs to be updated to point to the downloaded environment.

### Training and testing the agent

- The Continuous_Control.ipynb can be executed to train/test the agent. The agent checkpoint is saved in the folders single_arm_chkpt for single arm task and multi_arm_chkpt for multi arm task. You can skip the training part and directly jump to the last cell to load the checkpoint and see the trained agent perform the control task. Load the appropriate environments for the tasks before loading the checkpoints.

### Request

- I am building a library for doing reinforcement learning. The rllib folder is another embedded repository. It would be updated time to time. All my three projects are using the same repo. If you are interested in collaborating, you can fork it and contribute. I would be very grateful for your contributions.


