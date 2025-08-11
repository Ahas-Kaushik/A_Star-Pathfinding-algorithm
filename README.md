# Maze Solver 🤖

This project generates a random maze and uses the **A\* algorithm** to find and visualize the shortest path from a start point to a goal.



***

## How It Works

### Maze Generation
A new, unique maze is created every time you run the code. This is because it uses a **randomized algorithm** to carve out the paths. The `loopPercent=100` setting adds many extra routes, creating a complex grid rather than a simple labyrinth.

### Maze Solving: The A\* Algorithm
The maze is solved using **A\* (A-Star)**, a smart pathfinding algorithm. It's efficient because it doesn't search blindly. Instead, it intelligently prioritizes paths that seem to be leading closer to the goal.

It works by calculating a "cost" for each square using the formula: `f = g + h`
* **g**: The cost of the path from the start to the current square.
* **h**: The estimated cost from the current square to the end goal (the "heuristic").

A\* always explores the square with the lowest total cost `f`, which helps it find the shortest path quickly without wasting time on bad routes.

***

## The Visualization 🎨

The animation shows three different paths:

* 🔵 **Blue Agent**: Shows every single square the algorithm checked (the "search area").
* 🟡 **Yellow Agent**: Shows how the final path was constructed by backtracking from the goal.
* 🔴 **Red Agent**: Shows the final, optimal shortest path from start to finish.

***

## How to Run

### 1. Prerequisites
You need to install the `pyamaze` library.
```bash
pip install pyamaze
