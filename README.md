# Kakuro Game Solver
A Kakuro game solver created for AI: Reasoning &amp; Problem Solving class.

This Python project offers a Kakuro game solver that utilizes constraint propagation and backtracking to find solutions for Kakuro puzzles.
## Kakuro and it's rules
To learn more about the game visit the link here https://www.kakuros.com/

## How to Use

1. **Input Puzzle:** Define your Kakuro puzzle as a 2D list. Mark black cells as `'X'` and empty cells as `'.'` (periods). Provide horizontal and vertical constraints as lists of lists.
   
2. **Running the Solver:** Execute the `solve_kakuro()` function, passing the puzzle board, horizontal constraints, and vertical constraints. The solver will generate the solution for the given Kakuro puzzle.

## Code Overview

The code comprises several essential components:

- **Formatting Functions:** Functions to format and print the Kakuro board.
- **Board Class:** A class representing the Kakuro board, containing methods for constraint checking, constraint propagation, and solving the puzzle.
- **Main Solver:** The solver itself, implementing backtracking and constraint propagation to find the solution.
- **Testing:** An example puzzle is included for testing purposes.

## Functions and Classes

- `format_value`: Formats cell values for display.
- `pretty_print`: Prints the Kakuro board in a readable format.
- `create_cells_and_blocks`: Creates dictionaries of cells and blocks with their respective constraints.
- `Board` Class: 
  - `__init__`: Initializes the board.
  - `is_solved`: Checks if all block constraints are satisfied.
  - `consistent`: Checks if a value assignment is consistent with constraints.
  - `constraint_propagation`: Propagates constraints after assigning a value to a cell.
  - `update_due_to_backtracking`: Reverts the board state due to backtracking.
  - `find_most_constrained_empty_cell`: Finds the cell with the least options for value assignment.
  - Other helper functions for block identification and manipulation.

- `solve_kakuro`: Main function implementing the solver using backtracking and constraint propagation.

## Example

An example puzzle is included along with horizontal and vertical constraints for testing the solver.

## Running the Example

To test the solver on the provided example, execute the testing code provided at the end of the script.

Feel free to utilize this Kakuro game solver to solve your puzzles! If you have any inquiries or suggestions, contributions are welcome.


