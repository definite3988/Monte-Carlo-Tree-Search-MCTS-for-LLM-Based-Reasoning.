# 🏠 Monte Carlo Tree Search (MCTS) for the Zebra Puzzle

## 📌 Overview

This project implements **Monte Carlo Tree Search (MCTS)** to solve the **Zebra Puzzle**, a classic constraint satisfaction problem. The puzzle requires assigning five houses with different colors, nationalities, drinks, pets, and hobbies while satisfying a set of logical constraints.

## 🚀 How It Works

Monte Carlo Tree Search (MCTS) constructs a search tree where nodes represent **partial house assignments**. The algorithm follows these key steps:

1. **Selection**: Choose the most promising node using Upper Confidence Bound (UCT).
2. **Expansion**: Generate new states based on valid assignments.
3. **Simulation**: Randomly complete assignments while respecting constraints.
4. **Backpropagation**: Update wins and visits to improve future selections.

### 🧩 Constraints Enforced

The Zebra Puzzle follows **15 logical constraints**, such as:
- The **Englishman** lives in the **red house**.
- The **Spaniard** owns the **dog**.
- The **green house** is to the **right** of the **ivory house**.
- The **Norwegian** lives in the **first house**.
- The **Japanese person** plays **chess**.

MCTS eliminates invalid solutions early, ensuring only feasible states remain.
