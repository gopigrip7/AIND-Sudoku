# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: In the naked twins problem, the constraint is where any same two digits appear twice in the same units. Since two digits appear in the same unit, twice the constraint is these two digits cannot appear in any other boxes of the same units.This reduce the Sudoku problem to much solvable state and propagating this with elimination and only_once constraint reduce the problem to solved

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: This is much straight forward. The diagonal sudoku problem is much like normal sudoku where the constraint is the digits from 1 to 9 appear only ones in the left to right and right to left diagonals. This constraint is added to the unit list as one of the constraints. Eliminate, only_once and the naked_twin constraint are propagated the same way solving the diagonal problem.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in function.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
