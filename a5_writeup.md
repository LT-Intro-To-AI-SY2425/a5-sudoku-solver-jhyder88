# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?
I believe DFS is more efficient for sudoku specifically, due to there being a cap at how deep the search can go which doesn't allow for the chance of going to deep into a rabbit hole before shifting to another portion of the search. 
BFS is more preferable in a scenario in which their isn't a cap to how deep the DFS can go, which therefore means BFS is more preferred as it can spread out the search more at a shallower level, before eventually finidng the right option to go down.


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?



3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?
For larger scale operations, a more efficient version of either DFS or BFS likely needs to be used as it feels like we're pushing the limits of the search capabilities with this type of assignment. This assignment could be applied to the real world when looking at addressing managing options. When someone has multiple options for doing something, maybe deciding what to eat, they could go through different areas of search similar to DFS and BFS to find their most optimal solution.