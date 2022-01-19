# Snake Game - Reinforcement Q-Learning

**Complete Video Tutorial:** https://youtu.be/sTStp24Ujp8

# Project Information

The environment consists of two snakes (agents) and `4` food locations at any instant. The snakes (agents) can move in three directions; namely **left**, **right** or **straight** ahead. The objective of the game is to possess a greater score than the opponent either by consuming the food or by colliding with the opponent.

A breief description on the environment is given below:

### State Space:
- The state space is characterised by a `8 x 8` Grid (Continious Space).
- At any instant of time, `4` random coordinates out of `8` fixed coordinates possess food.

### Action Space:
- The agent may choose one of the three possible moves; left, right, forward at any instant.
- Depending on the position of the agent, the move may or may not be executed.
	- For instance, if the agent lies on the first row and is facing North, and decides to move left, the move will be determined illegal and the agent will not be displaced. Although the move does not take place, the agent will be turned to face West.
	- That is, the agent will first turn to left and then try to move. Since the move is illegal, the agent stays put.


### Rules:
1. The agent must eat the food to grow.
2. If the agent collides with the opponent:
	- Let `s1` and `s2` be the scores of the two agents. 
	- If `s1 > s2`, `r1 = 5 s2/(s1-s2)` and `r2 = -3 s2/(s1-s2)`
	- If `s1 < s2`, `r1 = -3 s1/(s2-s1)` and `r2 = 5 s1/(s2-s1)`
3. After collison, the agent with the lesser score is randomly respawned.

### Reward System:
- `-1` for legal moves
- `-2` for illegal moves
- `+4` for consuming food
- Collision
	- If `s1 > s2`, `r1 = 5 s2/(s1-s2)` and `r2 = -3 s2/(s1-s2)`
	- If `s1 <s 2`, `r1 = -3 s1/(s2-s2)` and `r2 = 5 s1/(s2-s1)`


# Libraries

- gym
- nqueens
- matplotlib
- opencv
- collections


# Algorithms

- Q-Learning