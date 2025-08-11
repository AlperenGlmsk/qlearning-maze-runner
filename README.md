# qlearning-maze-runner
An educational reinforcement learning project demonstrating Q-learning in a grid-based maze environment. Includes custom environment design, reward shaping, and epsilon-greedy policy implementation.

# Q-Learning Maze Runner 🧭🤖

A reinforcement learning project implementing a **Q-learning** agent to solve a grid-based maze.  
The agent learns optimal paths through trial-and-error, using an **epsilon-greedy** strategy to balance exploration and exploitation.

## 📌 Project Overview
This project demonstrates the fundamentals of **Reinforcement Learning (RL)** by teaching an agent to navigate a maze environment.  
Key features include:
- Customizable maze environment
- Q-table implementation from scratch
- Epsilon-greedy policy for exploration
- Reward shaping for faster convergence
- Visualization of agent's learning progress

## 🧠 Learning Approach
The agent:
1. Starts from a random position in the maze.
2. Chooses actions using an epsilon-greedy policy.
3. Receives rewards for reaching the goal and penalties for hitting walls.
4. Updates the Q-table using the Bellman equation.

**Q-learning Update Rule:**
```python
Q[state][action] = Q[state][action] + α * (reward + γ * max(Q[next_state]) - Q[state][action])

