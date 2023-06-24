# SnakeGame-using-RL
This project aims to develop an implementation of the classic Snake game using reinforcement learning techniques. Reinforcement learning is a subfield of machine learning that focuses on training agents to make decisions by rewarding or punishing them based on their actions. In this project, the snake game environment will be modelled as a Markov Decision Process (MDP), and an agent will be trained using a deep reinforcement learning algorithm to learn how to play the game. The performance of the trained agent will be evaluated by measuring its ability to maximize its score while avoiding collisions with the walls and its own tail. The project's ultimate goal is to demonstrate the feasibility of using reinforcement learning to develop agents capable of learning how to play simple games with minimal human intervention. 
We describe the design of the RL agent, including the state and action space, and reward signal. We used the Q-learning algorithm for training the agent, and experimented with different reward signals to optimize the agent's performance. Our experimental results show that the RL agent can successfully learn to play the snake game with high scores and outperform a baseline agent that uses a random policy.
![image](https://github.com/ckteja/SnakeGame-using-RL/assets/91280385/109bb977-f46e-4981-a66b-5a8532df75f0)
![image](https://github.com/ckteja/SnakeGame-using-RL/assets/91280385/43631108-4457-4ff4-8056-b710d1f5d4a4)

Methods and Techniques:
In the development of an autonomous snake game using reinforcement learning (RL), we used the following methods and techniques:
1. Q-Learning Algorithm:
 We used the Q-learning algorithm, which is a model-free RL algorithm, to train the agent. Q-learning is a temporal difference method that learns the optimal action-value function by iteratively updating the Q-values based on the reward received and the estimated Q-value of the next state.
2. Deep Q-Networks (DQN):
 To handle the high-dimensional state space of the snake game, we used a deep neural network as a function approximator to represent the Q-values. This approach is known as Deep Q-Networks (DQN) and has been shown to be effective in handling high-dimensional state spaces.
3. Experience Replay: 
To improve the stability of the learning process, we used experience replay, which involves storing and randomly sampling past experiences from a memory buffer. This allows the agent to learn from a diverse set of experiences and reduce the correlation between successive updates.
4. Epsilon-Greedy Exploration:
 To balance exploration and exploitation, we used an epsilon-greedy exploration strategy, where the agent selects a random action with a probability epsilon and the action with the highest Q-value otherwise. This allows the agent to explore new actions while also exploiting its current knowledge.
5. Reward Shaping: 
We experimented with different reward signals to optimize the agent's performance. We used a reward function that incentivized the agent to eat food, avoid obstacles, and stay alive for as long as possible. We also added a negative reward for actions that resulted in the game ending.
Overall, the combination of Q-learning, DQN, experience replay, epsilon-greedy exploration, and reward shaping allowed us to develop an RL agent that can play the snake game autonomously with high scores.
