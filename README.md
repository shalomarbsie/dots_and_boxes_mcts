# Dots and Boxes MCTS AI

An advanced Dots and Boxes game engine and AI player implemented using Monte Carlo Tree Search (MCTS). This project demonstrates how statistical simulations can master combinatorial games with complex turn-based logic.

## Features
- MCTS Engine: Implements Selection, Expansion, Simulation, and Backpropagation.
- UCB1 Logic: Balances exploration of new moves with exploitation of winning paths.
- Heuristic Rollouts: Logic in simulations to ensure high-quality data.
- Dynamic Visualization: Jupyter Notebook support with real-time board updates.
- Normalized Reward Scaling: AI prioritizes margin of victory rather than just binary wins.

## How the AI Works
The AI uses a Monte Carlo Tree Search algorithm to evaluate the best possible moves by simulating thousands of potential game outcomes.

The Core Loop:
1. Selection: Uses the UCB1 formula to navigate the search tree.
2. Expansion: Adds new potential moves to the tree.
3. Simulation: Plays a fast-forward version of the game using greedy heuristics.
4. Backpropagation: Updates the tree with the results of the simulation.

Optimizations:
- Transposition Tables: Hashes board states to avoid redundant calculations.
- Safe-Move Heuristics: Prevents the AI from making obvious mistakes during simulations.
- State Cloning: Optimized board copying to increase simulations per second.

## Usage
To watch two AIs compete, run the final cell in the Jupyter Notebook. You can adjust the board_size and the iterations parameter to change the difficulty.
