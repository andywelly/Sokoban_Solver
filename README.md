# Sokoban_Solver
AI solver for Sokoban puzzles, implemented in C

## What is Sokoban?

Sokoban is a classic puzzle game in which players control a warehouse worker whose objective 
is to push crates or boxes to designated storage locations within a maze-like environment.
The challenge lies in maneuvering the crates around obstacles and arranging them in the correct 
positions, all while avoiding getting trapped or creating unsolvable situations.

## [Visualisation](https://henrykautz.com/sokoban/Sokoban.html)


## Implementation

In this implementation of Dijkstra's algorithm for Sokoban puzzles, the game's state space is 
represented as a graph where nodes correspond to possible game states and edges represent valid
movements. By assigning costs to edges based on movement requirements, the algorithm efficiently
searches for the shortest path from the initial state to a goal state where all boxes are
correctly positioned on target destinations while considering constraints such as box movement
and obstacle avoidance. Through this approach, the solver can navigate the puzzle's state space to
find optimal solutions with minimal moves needed to achieve the objective.

## How to Use

In order to execute the AI solver use the following command:
./sokoban -s <map> play_solution

## Puzzle File Format

#: Wall<br/>
 : Space<br/>
.: Goal<br/>
@: Sokoban<br/>
$: Box<br/>
+: Sokoban on Goal<br/>
*: Box on Goal<br/>
%: Comment Line<br/>

## Solution File Format

l: Move Left<br/>
r: Move Right<br/>
u: Move Up<br/>
d: Move Down<br/>
L: Push Left<br/>
R: Push Right<br/>
U: Push Up<br/>
D: Push Down<br/>




