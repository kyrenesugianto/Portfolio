# Qlearning and Value Iteration 

In Project 3: Reinforcement Learning, I implemented various agents to solve Markov Decision Processes (MDPs) and tested them on Gridworld, a simulated robot controller (Crawler), and Pacman. Below is a summary of my contributions to each question:

I implemented a ValueIterationAgent, an offline planner that uses value iteration to compute k-step estimates of optimal values. The agent computes actions from values and Q-values based on the provided MDP. The batch version of value iteration was used, where each vector Vk is computed from a fixed vector Vk−1.

I explored different settings of discount, noise, and living reward parameters to produce optimal policies for specific scenarios in the DiscountGrid layout. I implemented settings that prefer the close or distant exit, with or without risking the cliff, and settings to avoid both exits and the cliff.

I implemented a Q-learning agent that learns from trial and error using the update method. The agent uses the Q-value update equation and explores the environment while updating its Q-values. I also implemented methods to compute values and actions from Q-values.

I completed the Q-learning agent by implementing epsilon-greedy action selection in the getAction method. The agent chooses random actions with a certain probability (epsilon) and follows the current best Q-values otherwise.

I tested the Q-learning agent in Pacman, where it learns a policy during training and exploits it during testing. I adjusted parameters such as epsilon, alpha, and gamma for effective learning and performance. The agent was evaluated based on its winning percentage in test games.

I implemented an ApproximateQAgent, a subclass of PacmanQAgent, which learns weights for features of states using the approximate Q-learning approach. The weight vector is updated based on the experienced reward and the difference between predicted and maximum Q-values. I used feature extractors to generalize learning across similar states.

Overall, my implementations involved understanding and applying reinforcement learning concepts, experimenting with different parameter settings, and ensuring correct interactions with the provided environments.






