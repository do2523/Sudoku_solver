# Sudoku Solver using Backtracking Algorithm

This Python program solves a Sudoku puzzle using a backtracking algorithm. It takes a partially filled 9 by 9 Sudoku grid as input and fills in the remaining empty cells to find a valid solution.

## How to Use

1. Ensure that you have Python 3 installed on your machine.

2. Clone this repository or download the source code file.

3. Open the terminal or command prompt and navigate to the project directory.

4. Run the `sudoku_solver.py` file using the Python interpreter.

5. The initial Sudoku grid is defined in the `board` variable within the code. Modify the `board` list to input your own Sudoku puzzle. Use '0' to represent empty cells.

6. After running the program, it will print the initial Sudoku grid.

7. The program will solve the Sudoku puzzle and print the solved grid if a solution is found.

## Backtracking Algorithm

The Sudoku solver uses a backtracking algorithm to find the solution. The algorithm follows these steps:

1. Find an empty cell in the Sudoku grid.

2. Try numbers from 1 to 9 in that cell.

3. Check if the number is valid according to Sudoku rules (no repetition in the same row, column, or box).

4. If the number is valid, place it in the cell and move to the next empty cell.

5. If a number is not valid or no number works, backtrack by undoing the previous placement and try the next number.

6. Repeat this process until a solution is found or all possibilities are exhausted.

## Example

The program includes an example Sudoku puzzle in the `board` variable. To solve a different puzzle, modify the `board` list accordingly.

Here's an example of a Sudoku puzzle input:

```python
board = [
    [7,8,0,4,0,0,1,2,0],
    [6,0,0,0,7,5,0,0,9],
    [0,0,0,6,0,1,0,7,8],
    [0,0,7,0,4,0,2,6,0],
    [0,0,1,0,5,0,9,3,0],
    [9,0,4,0,6,0,0,0,5],
    [0,7,0,3,0,0,0,1,2],
    [1,2,0,0,0,7,4,0,0],
    [0,4,9,2,0,6,0,0,7]
]
```

The program will output the solved Sudoku grid as follows:

```
7 8 5 4 3 9 1 2 6
6 1 2 8 7 5 3 4 9
4 9 3 6 2 1 5 7 8
5 2 7 1 4 3 2 6 8
8 6 1 7 5 2 9 3 4
9 3 4 1 6 8 7 9 5
2 7 8 3 9 4 6 1 2
1 2 6 5 8 7 4 9 3
3 4 9 2 1 6 8 5 7
```

## Contributions

Contributions to this project are welcome. If you find any issues or have suggestions for improvement, please feel free to submit a pull request.
