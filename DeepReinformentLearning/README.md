The following **intentional and justified changes** were made:

### 1️ Code Modularization
- Logic was reorganized into functions for:
  - Action selection
  - Q-value updates
  - Environment observation
- Improves readability and maintainability

---

### 2️ Fixed Action Selection Bug
- Corrected the action selection logic to properly use available actions
- EnsPrevented unintended global variable dependency

---

### 3️ Added ε-Greedy Exploration Strategy
- Introduced **ε-greedy policy** to balance:
  - Exploration (random action)
  - Exploitation (best known action)
- Makes learning more realistic and stable

---

### 4️ Preserved All Graph Visualizations ✅
The modified code **retains all important visual outputs** from the original implementation:

1. **Graph Structure Visualization**
   - Shows the connectivity of nodes using NetworkX

2. **Q-Learning Training Curve**
   - Plots reward vs number of iterations

3. **Graph with Environmental Labels**
   - Highlights police nodes, drug trace nodes, and target location

4. **Environment-Aware Learning Curve**
   - Shows learning behavior after incorporating environmental constraints

---

### 5️ Improved Environment Handling
- Environmental matrices created for:
  - Police encounters
  - Drug trace encounters
- Learning process adapts based on these observations

---

##  Algorithm Used
- **Reinforcement Learning**
- **Q-learning**
- **ε-greedy policy**
- Discount factor (γ) based future reward estimation

---

##  Output and Analysis
- Optimal path from start node to goal
- Reward convergence graphs
- Environmental influence matrices
- Comparison of learning before and after environment awareness

---

##  Technologies Used
- Python
- NumPy
- NetworkX
- Matplotlib / Pylab
- Reinforcement Learning concepts
