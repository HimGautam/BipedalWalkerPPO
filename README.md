# BipedalWalkerPPO
This project is based on Proximal Policy Optimization for continuous control task.

![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/70597091/164040478-a162bdbf-9bdb-4465-930a-078ddd9f11db.gif)

# Overview
In this project we solve BipedalWalker problem of OpenAI Gym using PPO algorithm. I've used my [ppo-cartpole](https://github.com/HimGautam/ppo-cartpole) work as a reference to this work. The algorithm used in this work is same with a few adjustments in HyperParameters, Input and Output Dimension of NN.

It took 10_00_000 training steps using the my set of hyperparameters to achieve the performance shown above. You can also experiment with the hyperparameters to see if you can get some improvements.

# Requirements
 
 This code requires following dependencies:
 
 1) Jupyter Notebook
 2) Python
 3) Open AI Gym
 4) Numpy
 5) Tensorflow
 6) Tensorflow-Probability
 7) Tensorboard

# Trying Out

You can either train the NN by your own or you can use weights from my training to see the results I have achieved. Just place [actor.hdf5](https://github.com/HimGautam/BipedalWalkerPPO/blob/main/actor.hdf5), [critic.hdf5](https://github.com/HimGautam/BipedalWalkerPPO/blob/main/critic.hdf5) and [log_std](https://github.com/HimGautam/BipedalWalkerPPO/blob/main/log_std.hdf5) in the same folder with [BipedalPPO.ipynb](https://github.com/HimGautam/BipedalWalkerPPO/blob/main/BipedalPPO.ipynb). Use ```agent.load()``` after initialization of agent to load the weights and then run the last with ```#Testing``` comment.

For training the agent by yourself, don't load the weights and run the cell with ```Training``` comment.
