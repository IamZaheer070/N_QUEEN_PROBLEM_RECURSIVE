# N-Queens Problem

This project provides a solution to the N-Queens problem using a recursive approach. The N-Queens problem involves placing N queens on an N x N chessboard such that no two queens threaten each other. The solution is implemented using Python and demonstrates the use of recursion and backtracking.

## Code Overview

1. **Initialization:**
   - `numQueens`: The number of queens to place on the board (default is 8).
   - `currentSolution`: A list to hold the current configuration of the board.
   - `solutions`: A list to store all the valid solutions found.

2. **Safety Check (`isSafe` function):**
   - Checks if placing a queen at the given row and column is safe by:
     - Ensuring no other queen is placed in the same column.
     - Ensuring no other queen is on the same diagonal.

3. **Queen Placement (`placeQueen` function):**
   - Recursively attempts to place queens in each column of the current row.
   - If placing a queen results in a solution, it is added to the `solutions` list.
   - Continues to the next row until all rows are processed or all solutions are found.

4. **Execution:**
   - Starts solving the problem by calling `placeQueen` for the first row.
   - Outputs the number of solutions found and prints each solution.
