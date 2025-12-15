# Tic-Tac-Toe using Reinforcement Learning

This project implements a **Tic-Tac-Toe game using Reinforcement Learning** where an AI agent learns optimal strategies by playing repeated games.  
The agent is trained using **state-value updates** and later plays against a human player.

---

##  Objective
To apply **reinforcement learning principles** for training an intelligent agent that can learn to play Tic-Tac-Toe optimally without explicit rules.

---

##  Original Code Overview
The original implementation:
- Used a basic RL agent
- Stored state values using a dictionary
- Allowed AI vs AI training
- Supported Human vs AI gameplay

---

##  Modifications Made (IMPORTANT)

The following meaningful changes were introduced:

### 1️ Bug Fixes
- Corrected player initialization logic
- Fixed symbol assignment inconsistencies

### 2️ Improved Training Structure
- Modularized training loop
- Cleaner game state reset handling

### 3️ Enhanced Reward Strategy
- Balanced reward values for win, loss, and draw
- Improved convergence stability

### 4️ Improved Readability
- Clearer variable naming
- Added comments for understanding flow

### 5️ Policy Persistence
- Trained policy is saved and loaded using `pickle`
- Enables reuse of trained AI without retraining

---

##  Algorithm Used
- Reinforcement Learning
- State-value function approximation
- Exploration vs Exploitation strategy

---

##  Gameplay Modes
- AI vs AI (training)
- Human vs AI (interactive play)

---

##  Technologies Used
- Python
- NumPy
- Pickle (for policy persistence)
- Reinforcement Learning concepts
