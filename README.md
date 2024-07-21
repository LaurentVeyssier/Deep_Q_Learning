# Deep_Q_Learning
Reinforcement learning with Deep Convolutional Q Learning model 

This project is taken from [Udemy]()

# Project Description

We will use a deep convolutional Q Learning model to train a model on PacMan.
The Atari PacMan game is obtained through gymnasium package, itself derived from OpenAI gym library for reinforcement learning.

Our objective is to train a DCQN model to play PacMan using reinforcement learning.
Images are fed to the model which predicts the action to implement.

# DCQM Model design

The model will be composed of 4 CNN blocks (Convolution layer followed by a batch normalization step and a ReLU rectifier). After a flattening step, the signal will feed into a fully dense neural net with 2 layers.
- model input = game-generated RGB images of resolution 210 x 160 transformed to 128 x 128 RGB images
- model output = vector with size equal to the number of possible actions (9 in total)

# Reinforcement learning algorithm

- Agent with local and target DCQ networks
- replay memory
- epsilon greedy action selection from the model output

# results

The agent was trained up to a low score of 400 for demonstration purpose.
Much longer training is required to achieve decent performance.

![](pacman_video.mp4)
