# Graph Coloring 

## Overview
This is a Python-based desktop application for solving the graph coloring problem using **Backtracking** and **Genetic Algorithm**. It features a graphical user interface (GUI) built with Tkinter, allowing users to create graphs, specify edges, and visualize the colored results using NetworkX and Matplotlib.

## Features
- **Graph Creation**: Input the number of nodes and edges, and define edge connections.
- **Algorithm Options**: Choose between Backtracking or Genetic Algorithm to color the graph.
- **Visualization**: Displays the graph with nodes colored to avoid adjacent conflicts.
- **Performance Tracking**: Shows the execution time for the selected algorithm.
- **Error Handling**: Validates inputs and alerts users to invalid entries or algorithm timeouts.

## Requirements
- Python 3.x
- Required libraries:
  - `networkx`
  - `numpy`
  - `matplotlib`
  - `tkinter` (included with Python)

Install dependencies:
```bash
pip install networkx numpy matplotlib
```

## Project Structure
- `main.py`: Implements the `GraphOperations` class and algorithms (Backtracking and Genetic).
- `gui.py`: Defines the Tkinter GUI and integrates graph creation and visualization.
- `README.md`: This file, providing project details and instructions.

## Example
For a graph with 4 nodes and 3 edges:
- Nodes: `4`
- Edges: `3`
- Edge connections:
  ```
  1,2
  2,3
  3,4
  ```
- Select an algorithm and click "Create and Solve".

## Algorithm Details
- **Backtracking**: Assigns colors incrementally, backtracking on conflicts. Times out after 5 seconds for complex graphs.
- **Genetic Algorithm**: Evolves a population (size: 50, generations: 1000, mutation rate: 0.01) to minimize coloring conflicts.
