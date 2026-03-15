# Single-Point Metaheuristic Algorithms for NP-Hard Problems
## Overview

This project explores the application of **single-point metaheuristic optimization algorithms** to solve classical **NP-hard combinatorial optimization problems.** The goal of the study was to evaluate how different local-search based algorithms perform when solving computationally difficult optimization tasks.

The project focuses on analyzing the effectiveness of several **single-solution search algorithms** and comparing their performance in terms of **solution quality, convergence behavior, and computational efficiency.**

The implementation and experiments were conducted using **Python in Google Colab.**

## Problems Studied
### 1. Knapsack Problem

The Knapsack Problem is a well-known combinatorial optimization problem where the objective is to select a subset of items with given weights and values in order to maximize the total value while keeping the total weight within a specified capacity.

Because the number of possible item combinations grows exponentially with the number of items, the problem becomes computationally difficult for large instances.

### 2. Partition Problem

The Partition Problem involves dividing a set of integers into two subsets such that the difference between their sums is minimized.

This problem is also classified as NP-hard, making exact solutions impractical for larger datasets and motivating the use of metaheuristic optimization algorithms.

## Algorithms Implemented

The project focuses on single-point search algorithms, which iteratively improve a single candidate solution rather than maintaining a population of solutions.

The following algorithms were implemented and evaluated:

### Tabu Search (TS)

Tabu Search uses a memory-based approach to avoid revisiting previously explored solutions. A tabu list prevents the search from cycling and helps escape local optima.

### Simulated Annealing (SA)

Simulated Annealing is inspired by the annealing process in metallurgy. The algorithm probabilistically accepts worse solutions during early iterations to escape local optima and gradually focuses on better solutions.

### Iterated Local Search (ILS)

Iterated Local Search repeatedly applies local search while introducing perturbations to the current solution to explore new regions of the search space.

### Guided Local Search (GLS)

Guided Local Search introduces penalties to frequently used solution features to guide the search toward unexplored areas of the solution space.

## Hyperparameter Optimization

To improve algorithm performance, hyperparameter optimization was performed using the Optuna framework.

The optimization process was used to tune parameters such as:

- cooling schedule parameters in Simulated Annealing

- tabu list size in Tabu Search

- perturbation strength in Iterated Local Search

- penalty control parameters in Guided Local Search

This allowed the algorithms to achieve improved solution quality across multiple test instances.

## Experiments and Evaluation

The algorithms were evaluated through experiments on generated problem instances. Performance was analyzed based on several factors:

- quality of the final solution

- convergence behavior of the algorithms

- computational efficiency

The results demonstrate how different metaheuristic strategies perform when applied to complex optimization problems.

## Technologies Used

**Programming Language**
- Python

**Libraries and Tools**
- Optuna (Hyperparameter Optimization)
- Google Colab

**Concepts and Methods**
- Metaheuristic Optimization
- Single-Point Search Algorithms
- Combinatorial Optimization
- Algorithm Performance Analysis

## Running the Project

This project was developed and executed using Google Colab.

To run the notebook:

1. Open the .ipynb file in Google Colab.

2. Run the notebook cells sequentially to reproduce the experiments and results.

## Learning Outcomes

Through this project, the following concepts were explored:

- application of metaheuristic algorithms to NP-hard problems

- comparison of different single-point search strategies

- hyperparameter optimization using Optuna

- analysis of algorithm convergence behavior

## Future Improvements

Possible future improvements include:

- applying the algorithms to additional NP-hard problems

- comparing single-point search algorithms with population-based methods such as Genetic Algorithms and Ant Colony Optimization

- extending the experiments to larger datasets

- developing visualization tools for algorithm convergence behavior
