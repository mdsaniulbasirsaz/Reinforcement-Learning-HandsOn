## What is Reinforcement Learning?
Think of Reinforcement Learning as learning by trial and error. An agent interacts with an environment, takes actions, receives rewards, and gradually learns the best behavior.

# 1. Agent

The **Agent** is the decision-maker.

### Responsibilities:
- Observes the environment
- Takes actions
- Learns from rewards

### Example:
- Delivery robot control system
- Game-playing AI

---

# 2. Environment

The **Environment** is everything the agent interacts with.

### It:
- Responds to actions
- Provides next state
- Gives reward signals

### Example:
- Roads
- Traffic
- Obstacles
- Buildings

---

# 3. State (S)

The **State** represents the current situation of the environment.

### Example:
- Robot position
- Distance to target
- Obstacles nearby


S_t = environment representation at time t


---

# 4. Action (A)

The **Action** is what the agent does in a state.

### Example:
- Move forward
- Turn left/right
- Stop


A_t = action taken at time t


---

# 5. Reward (R)

The **Reward** is feedback from the environment.

### Purpose:
- Positive reward → good action
- Negative reward → bad action

### Example:
- +10 → successful delivery
- -1 → collision risk

Goal: maximize total reward

---

# 6. Policy (π)

The **Policy** defines the agent’s behavior.


π: State → Action


### Types:
- Deterministic policy
- Stochastic policy

In deep RL:
- Implemented using neural networks

---

# 7. Value Function

The **Value Function** measures how good a state or action is.

### State Value:

V(s)


### Action Value (Q-function):

Q(s, a)


Used in:
- Q-learning
- Deep Q Networks (DQN)

---

# 8. Reinforcement Learning Loop

Observe state S_t
Choose action A_t (policy π)
Execute action
Receive reward R_t
Get next state S_{t+1}
Update policy/value function

---

# 9. Exploration vs Exploitation

### Exploration:
- Try new actions
- Learn more about environment

### Exploitation:
- Use best known action
- Maximize reward

Trade-off is key in RL.

---

# 10. Goal of RL

Maximize long-term cumulative reward:


Max Σ (future rewards)