# Using Deep Reinforcement Learning to Solve Acrobot

**NOTE**: This project was done a long time ago when I first started with reinforcement learning, so please excuse some conceptual inaccuracies, e.g. I'm not actually using the DDPG algorithm, and I'm not doing the "asynchronous" part of A3C :) Otherwise, I *am* using policy gradients with actor/critic networks, with advantage (A2C).

This project uses policy gradients with actor/critic networks and parallel environments to solve OpenAI Gym's Acrobot-v1 environment. As of September 20, 2016, the final learned model placed 3rd on the OpenAI Gym Acrobot-v1 leaderboard, with a score of -80.69 ± 1.06 (see "georgesung's algorithm"): https://gym.openai.com/envs/Acrobot-v1

This project is my capstone project for Udacity's Machine Learning Engineer Nanodegree. For the full capstone project report, please see 'Report.pdf'.

## Dependencies
The following depenencies are required:

* Python 2.7/3.5+
* NumPy
* Matplotlib
* OpenAI Gym
* TensorFlow 0.10.0

## How to run
To run the learning agent with pre-set parameter values, run 'python learning_agent.py'. The main reinformcent learning code is located in this file.

To run the parameter search, run 'python search_params.py'. In this file, you can modify the parameter values over which to search.

Once you know your optimal parameters, enter them in 'full_training.py', and run 'python full_training.py'. This will perform the full training process on the model.

To validate your model (make sure results are consistent), run 'python model_eval.py'.

## Detailed report
A full detailed report can be found at 'Report.pdf'

## Final model
My final trained model is available at 'models/model.ckpt'. This model is saved as a TensorFlow model.
