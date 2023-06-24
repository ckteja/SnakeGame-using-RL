# SnakeGame-using-RL
This project aims to develop an implementation of the classic Snake game using reinforcement learning techniques. Reinforcement learning is a subfield of machine learning that focuses on training agents to make decisions by rewarding or punishing them based on their actions. In this project, the snake game environment will be modeled as a Markov Decision Process (MDP), and an agent will be trained using a deep reinforcement learning algorithm to learn how to play the game. The performance of the trained agent will be evaluated by measuring its ability to maximize its score while avoiding collisions with the walls and its own tail. The project's ultimate goal is to demonstrate the feasibility of using reinforcement learning to develop agents capable of learning how to play simple games with minimal human intervention. 
We describe the design of the RL agent, including the state, action space, and reward signal. We used the Q-learning algorithm for training the agent and experimented with different reward signals to optimize the agent's performance. Our experimental results show that the RL agent can successfully learn to play the snake game with high scores and outperform a baseline agent that uses a random policy.
![image](https://github.com/ckteja/SnakeGame-using-RL/assets/91280385/cc681a15-1371-4e0a-9128-f7a452ca9d18)


![image](https://github.com/ckteja/SnakeGame-using-RL/assets/91280385/62f7c9eb-f512-4295-a9d7-ee7e23f0f753)


## Methods and Techniques Used:

### Q-Learning Algorithm:
 We used the Q-learning algorithm, a model-free RL algorithm, to train the agent. Q-learning is a temporal difference method that learns the optimal action-value function by iteratively updating the Q-values based on the reward received and the estimated Q-value of the next state.
### Deep Q-Networks (DQN):
 To handle the high-dimensional state space of the snake game, we used a deep neural network as a function approximator to represent the Q-values. This approach is known as Deep Q-Networks (DQN) and has been shown to be effective in handling high-dimensional state spaces.
### Experience Replay: 
To improve the stability of the learning process, we used experience replay, which involves storing and randomly sampling past experiences from a memory buffer. This allows the agent to learn from a diverse set of experiences and reduces the correlation between successive updates.
### Epsilon-Greedy Exploration:
 To balance exploration and exploitation, we used an epsilon-greedy exploration strategy, where the agent selects a random action with a probability epsilon and the action with the highest Q-value otherwise. This allows the agent to explore new activities while also exploiting its current knowledge.
### Reward Shaping: 
We experimented with different reward signals to optimize the agent's performance. We used a reward function that incentivized the agent to eat food, avoid obstacles, and stay alive for as long as possible. We also added a negative reward for actions that resulted in the game ending.

Overall, the combination of Q-learning, DQN, experience replay, epsilon-greedy exploration, and reward shaping allowed us to develop an RL agent that can play the snake game autonomously with high scores.
