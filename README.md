# 🎲 Reinforcement Learning in Chutes and Ladders & Other Games  

## 📌 Project Overview  
This project applies **reinforcement learning (RL)** techniques to solve stochastic board games, with a primary focus on **Chutes and Ladders**. The implementation explores different RL algorithms, including:  
- **Dynamic Programming**  
- **Monte Carlo Methods**  
- **SARSA (State-Action-Reward-State-Action) Learning**  
- **Q-Learning**  

Additionally, the project extends reinforcement learning concepts to solve other probabilistic games, such as:  
- **The Coin Flip Game** (optimal decision-making under risk)  
- **Hi Ho Cherry-O** (estimating expected turns to victory)  

## 🎯 Objective  
The goal of this project is to analyze how different RL strategies can optimize decision-making in stochastic environments, focusing on policy optimization and value estimation in uncertain game scenarios.  

---

## 🏗️ Methodologies  

### 1️⃣ **Dynamic Programming**  
**Approach:**  
- Defines a **state-space** representation for the Chutes and Ladders game.  
- Uses **Bellman equations** to iteratively improve a value function.  
- Computes the optimal policy by **local search** over possible actions (dice choices).  

**Outcome:**  
- Generates an optimal policy that minimizes the expected number of moves to reach the goal.  

### 2️⃣ **Monte Carlo Learning**  
**Approach:**  
- Simulates **gameplay trajectories** to collect experience.  
- Uses **returns from simulated games** to update state-action values.  
- Implements **ε-greedy exploration** to balance exploration and exploitation.  

**Outcome:**  
- Estimates the **best dice choice** at each state to reach the goal in the shortest time.  
- Provides a **policy visualization** to map optimal actions on the game board.  

### 3️⃣ **SARSA (On-Policy TD Learning)**  
**Approach:**  
- Learns **Q-values** by updating state-action pairs using TD (Temporal Difference) updates.  
- Incorporates **ε-greedy exploration** to balance learning and optimality.  
- Uses a **stepwise update rule** to refine action choices dynamically.  

**Outcome:**  
- A robust policy that adjusts dynamically based on exploration-exploitation balance.  

### 4️⃣ **Q-Learning (Off-Policy TD Learning)**  
**Approach:**  
- Similar to SARSA but follows a more aggressive strategy by always **picking the highest-value action**.  
- Uses a **max-Q update rule** for better convergence.  
- Applies **discounted rewards** to optimize long-term gains.  

**Outcome:**  
- Provides an **alternative RL policy** that often converges faster but is less exploratory than SARSA.  

---

## 🎮 Applications Beyond Chutes and Ladders  

### 🪙 **Coin Flip Game (Risk Management Strategy)**  
- A player has three turns to **flip a coin or pass**.  
- Flipping risks losing all accumulated money, while passing secures current earnings.  
- Monte Carlo learning helps determine **optimal risk-taking strategies** to maximize expected value.  

### 🍒 **Hi Ho Cherry-O (Turn Optimization)**  
- A stochastic game where a player spins a wheel to either **gain or lose cherries**.  
- Monte Carlo methods estimate the **expected number of turns** needed to win.  
- Helps analyze probabilistic decision-making with **random event chains**.  

---

## 📊 Visualization & Analysis  
The project includes **graphical representations** of RL strategies using:  
✅ **State vs. Value Function Plots** – Displays how states are valued over time.  
✅ **Optimal Policy Heatmaps** – Maps out the best moves based on RL learning.  
✅ **Game Board Visualizations** – Color-coded grids representing RL-driven policies.  

---

## 🧠 Key Insights  
📌 **Monte Carlo methods** perform well in highly stochastic environments but require many episodes to converge.  
📌 **Q-Learning** finds **greedy optimal policies** but may miss exploratory opportunities.  
📌 **SARSA** balances exploration and exploitation better than Q-Learning.  
📌 **Dynamic Programming** is effective but requires a fully known model of state transitions.  

---

## 📖 References  
This project is inspired by reinforcement learning concepts outlined in **Sutton & Barto’s "Reinforcement Learning: An Introduction"**.  

---

## 👥 Contributors  
- **Andrew Angulo**  
- **Liam Quinlan**  
- **Daniel Ziabicki**  
