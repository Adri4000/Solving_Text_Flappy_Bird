# Solving Text Flappy Bird with Reinforcement Learning Algorithms

The aim of this repository is to solve the Text Flappy Bird (TFB) environment, using a constant step-size Monte Carlo, and of a Sarsa($\lambda$) agents.

## Text Flappy Bird for OpenAI Gym

This repository contains the implementation of two OpenAI Gym learning environments of a simple unit-element player version of the Flappy Bird. The code base is heavily borrows from the [flappy-bird-gym](https://github.com/Talendar/flappy-bird-gym) repository.

It is inspired by the NetHack game and can be rendered within a terminal using simple character elements. The two environments differ only in the yielded observations. The `TextFlappyBird-screen-v0` returns the array that represents the current state of the game screen encoded as integers while the `TextFlappyBird-v0` returns the horizontal and vertical distance of the player to the closest upcoming pipe gap.

## Solving the environment with RL algorithms

This repository also contains a Jupyter Notebook, where there are the implementation of a constant step-size Monte Carlo, and of a Sarsa($\lambda$) agents. Both of these agents can solve the `TextFlappyBird-screen-v0` and `TextFlappyBird-v0` environments, as they are trained by considering as state space the horizontal and vertical distance of the player to the closest upcoming pipe gap. The notebook also explores a comparison between the two agents, highlighting their respective advantages and drawbacks.