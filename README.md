# AI_Reinforced_Learning_Quadcopter

# Project Overview

In this project I try to train a neural network algorithm to fly a quadcopter. The physics of the quadcopter are simulated so
that no real vehicle has to be used. The algorithm has the task to start the quadcopter vertical by taking control of the rotors. This is a done by a reinforced learning algorithm.

# Packages

For this jupyter notebook to run you need these common packages: Pyhton 3.6, jupyter notebook, numpy, matplotlib, keras.

# Files

physics_sim.py: python file which simulates the physics for a quadcopter.

task.py: python file which defines the task to be learned, the reward function and the next state.

agents directory: agent_solution.py imports the functions from the other python files in this directory  and is the agent
                  which learns the task. The replay buffer will provide a batch of experiences, the actor and the critic are
                  two neural networks which are trained and OUNoise is an exploration noise which helps the learning process
                  in finding directions.


# Conclusion, Findings

I was able to teach the quadcopter to start vertically. It was achieved with Deep Deterministic Policy Gradient. It has to
be acknowledged, that the physics_sim.py was the environment to learn for the agent and not a real quadcopter. The main 
difficulty after finding a model architecture is to define a reward function.

# Licensing, Authors, Acknowledgements

This repository is licensed under the MIT-License. Big thanks to udacity for providing the data and the code to start.
