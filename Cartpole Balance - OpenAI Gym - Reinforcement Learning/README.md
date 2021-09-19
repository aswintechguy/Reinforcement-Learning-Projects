# CartPole Balance - OpenAI Gym - Reinforcement Learning

**Complete Video Tutorial:** https://youtu.be/7SVv07QXO5M

# Project Information

A pole is attached by an un-actuated joint to a cart, which moves along a frictionless track. The system is controlled by applying a force of +1 or -1 to the cart. The pendulum starts upright, and the goal is to prevent it from falling over. A reward of +1 is provided for every time step that the pole remains upright. The episode ends when the pole is more than 15 degrees from vertical, or the cart moves more than 2.4 units from the center.

Observation:
        Type: Box(4)
        Num     Observation               Min                     Max
        0       Cart Position             -4.8                    4.8
        1       Cart Velocity             -Inf                    Inf
        2       Pole Angle                -0.418 rad (-24 deg)    0.418 rad (24 deg)
        3       Pole Angular Velocity     -Inf                    Inf
    Actions:
        Type: Discrete(2)
        Num   Action
        0     Push cart to the left
        1     Push cart to the right


**Install Modules** 
> pip install gym stable_baselines3

# Libraries

<li>gym
<li>stable_baselines3
<li>pytorch


# Algorithms

<li>PPO
	<li>MlpPolicy
  
**Best Model Score:** 200 (Highest Score)