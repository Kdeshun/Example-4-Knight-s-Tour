Pictures – 
 ![image](https://github.com/Kdeshun/Example-4-Knight-s-Tour/assets/122183169/83fe222a-2d28-44a7-a7fb-ffc1cadf4697)
 ![image](https://github.com/Kdeshun/Example-4-Knight-s-Tour/assets/122183169/ca19067d-c786-4ca4-9f57-5a1a72482aee)
 ![image](https://github.com/Kdeshun/Example-4-Knight-s-Tour/assets/122183169/3a1af90c-7af5-4ac9-bcc0-b358206a819b)
 ![image](https://github.com/Kdeshun/Example-4-Knight-s-Tour/assets/122183169/5354bfc3-68a7-4c93-b00e-20ca5d36f11d)
 ![image](https://github.com/Kdeshun/Example-4-Knight-s-Tour/assets/122183169/38809cb6-aeb1-411a-ad14-9b7c1278e7b4)
The program I’ve developed is a C# implementation of the Knight's Tour issue. The Knight's Tour is a mathematical problem in which the aim is to identify a set of movements for a knight on a chessboard that allows the knight to visit every square precisely once.
Here's a rundown of what's going on in the program:

1. The chessboard is shown as a grid, with the size set to 8x8 (BoardSize = 8).

2. The software creates an array to hold the knight's probable moves in the x and y directions (xMove and yMove).

3. All squares on the chessboard are marked as unvisited (-1).

4. The beginning point of the knight is set to (0, 0), and this place is noted as visited (0).

5. To begin solving the Knight's Tour issue, the solveKT function is invoked.

6. The chessboard is initialized and the beginning point is registered as visited in the solveKT function.

7. The application begins recursive backtracking by calling the solveKTUtil method. It publishes the answer if one is discovered; else, it prints "No solution exists."
8. The backtracking algorithm is built on the solveKTUtil function. It is given the current location (x, y) and the number of moves. It also records attempted motions.
9. A solution is discovered and the method returns true if the move count approaches the entire number of squares on the chessboard.
10. The computer provides a list of potential moves for the knight. It evaluates unvisited squares and sorts them in ascending order depending on the number of unvisited neighbors.
11. It iterates through the ordered potential moves, marking each move on the board and invoking solveKTUtil recursively for the next move.
12. If a solution for the next move is discovered, it returns true. Otherwise, it reverts to the unvisited state and proceeds to the next potential step.
13. If no solution from the present point is discovered, the method returns false.
14. The CountVisitedNeighbors function counts the number of neighbors who have visited a particular square. It determines whether or not the square is a valid unvisited square for a knight's move.
15. The isSquareSafe function determines if a square is inside the chessboard limits and whether it has been visited.
16. After the Knight's Tour, the printSolution function is used to print the final solution or the board state.
Backtracking is used by the algorithm to investigate all potential knight movements in order to find a sequence that reaches every square precisely once. To discover the answer, it employs a depth-first search strategy. The application also records attempted movements for optimization purposes. The outcomes are shown on the console.
![image](https://github.com/Kdeshun/Example-4-Knight-s-Tour/assets/122183169/06a0f6ab-2315-422c-8ea1-1ba25cdd8c90)
