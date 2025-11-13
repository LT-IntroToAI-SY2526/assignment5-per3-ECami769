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

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?
I learned about the concept of backtracking and using "pop" to remove the stack and then search it and then fidning the most constrained cell and then putting it back in with multiple in one stack. I think a challenge that I faced while trying to implement these was finding the difference between DFS and BFS, I understood the concept of how they were different and the slide show helped it put it into visuals for me but I struggled to find the right way to code it, especially since they are similar it was harder to figure out what about the code was going to be different.


2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?
I think other games that could use this code are games like chess, checkers and probably more board games similar to those bceause these games are a process of thinking thorugh mutiple options of where to go, and then having to "recover" from the response of the other player and react to the situation apporpriately which would decide where you place the next piece.


3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?
DFS uses LIFO which means that it goes deeper first, which explains the name depth first search. DFS would use a stack becuase it follows one path as far as it can which means it needs a stack, while BFS would use a queue because they are different because BFS explores all the things at the current level, revealing that it needs different data structure. BFS would use FIFO because it is a breadth level search. 