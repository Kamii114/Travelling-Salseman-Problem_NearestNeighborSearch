# Traveling Salesman Problem and Nearest Neighbor Search

## Overview

This repository contains Jupyter notebooks that explore two significant optimization problems: the Traveling Salesman Problem (TSP) and the Nearest Neighbor Search (NNS). Both algorithms are essential in various fields such as logistics, routing, and network design.

## Problem Background

### Traveling Salesman Problem (TSP)

The TSP is a classic optimization problem that seeks to determine the shortest possible route visiting a set of points exactly once and returning to the starting point. The problem is NP-hard, meaning that finding an exact solution becomes increasingly difficult as the number of points grows. The origins of TSP date back to the 1800s and have applications in logistics, planning, and the manufacturing of microchips.

### Nearest Neighbor Search (NNS)

NNS is an optimization technique used to find the closest point from a given set of points. The problem became prominent with the development of spatial data structures and algorithms in the 1970s. NNS is widely used in various applications, including pattern recognition, image retrieval, and machine learning.

## Repository Contents

This repository includes two notebooks that implement both algorithms using brute-force approaches:

### Nearest Neighbor Search Notebook

- **Algorithm Overview**: This notebook implements a brute-force version of the NNS algorithm with a time complexity of \(O(n^2)\). It iteratively selects the nearest unvisited point based on a distance matrix built from the Euclidean distances between 2D points.
- **Key Steps**:
  1. Loading and preparing the dataset.
  2. Calculating Euclidean distances between the points.
  3. Implementing the NNS algorithm to find the optimal path.
  4. Measuring the execution time of the process.
  5. (Optional) Visualizing the NNS path using the `igraph` library.
  
- **Conclusion**: The NNS algorithm successfully finds the shortest path in a set of 2D points. While effective for small datasets, its quadratic time complexity may limit performance for larger datasets. Future optimizations or alternative approaches could enhance scalability.

---

### Traveling Salesman Problem Notebook

- **Algorithm Overview**: This notebook implements a brute-force solution to TSP with a time complexity of \(O(n!)\). The algorithm evaluates all possible permutations of the points to find the optimal tour based on the distances calculated from a distance matrix.
- **Key Steps**:
  1. Loading and preparing the dataset of 2D points.
  2. Calculating Euclidean distances between the points to create a distance matrix.
  3. Implementing the brute-force TSP algorithm to find the optimal tour and its cost.
  4. Measuring the execution time of the entire process.
  5. (Optional) Visualizing the tour using the `igraph` library.
  
- **Conclusion**: The TSP algorithm efficiently finds the optimal solution for smaller datasets by calculating all possible tours. However, its factorial time complexity makes it impractical for larger datasets. Future work could explore heuristic or approximation algorithms to improve scalability.

## Execution and Visualization

The notebooks include built-in timers to measure execution time and optional visualizations of the paths using the `igraph` library. These visual representations provide an intuitive understanding of the solutions.

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/repository_name.git
