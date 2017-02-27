# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: We find the boxes that have same value and the value length is 2 in unit, then remove the digits from the other box that in the same unit. so no other box in their
   same unit can contain the same digits and no squares outside the two naked twins squares can contain the twin values.
   For example, there are twins in the same column which contain the digit 2 and 3, namely there are two boxes who have same value {2,3} in the column, then we can eliminate the 
   digit 2 and 3 from the other boxes that in the same column, thus we reduce the occurrence probability of digit 2 or 3 and solve the sudou more faster.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: There are two diagonals, each has 9 boxes, we fill each diagonal of grid with all of the digits from 1 to 9.
    Just like we add constraint propagation to the row, column or square, we make the boxes in the same diagonal have the numbers from 1 to 9 only once.

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

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
