# N-Queens-II-leet6

Problem Description
The N-Queens puzzle is the problem of placing N queens on an N x N chessboard such that no two queens can attack each other. The task is to find the number of distinct solutions to the N-Queens puzzle.

Example
Input: n = 4

Output 2


Explanation:
For N = 4, there are two distinct solutions to the N-Queens puzzle, as shown below:

Solution 1:

. Q . .
. . . Q
Q . . .
. . Q .


Solution 2:

. . Q .
Q . . .
. . . Q
. Q . .


_**Approach**_
To solve the N-Queens puzzle, we can use a backtracking algorithm. The steps of the approach are as follows:

Create an N x N chessboard represented as a 2D grid.
Start solving the puzzle from the first row, trying to place a queen in each column of the current row.
Check if placing a queen at a specific position is valid by checking for conflicts with previously placed queens in the same column, upper left diagonal, and upper right diagonal.
If a valid position is found, place the queen at that position and move to the next row.
Repeat steps 3 and 4 recursively until all rows are filled with queens or a conflict is detected.
If all rows are filled with queens (a solution is found), increment the count of distinct solutions.
Backtrack by removing the queen from the current position and continue exploring other possibilities.
Return the count of distinct solutions.


_**Time Complexity Analysis**_

The time complexity of this solution is O(N!) as there are N! possible configurations to check.



_**Space Complexity Analysis**_

The space complexity is O(N) as we are using a 2D grid to represent the chessboard and the recursive call stack.


Summary

The "N-Queens" problem is about finding the number of distinct solutions to place N queens on an N x N chessboard without any two queens attacking each other. By using a backtracking algorithm, we can efficiently explore different configurations and find valid solutions. The solution has a time complexity of O(N!) and a space complexity of O(N).

Please make sure to provide a valid input value for N and include the necessary headers to run the code successfully.

Feel free to reach out if you have any further questions or clarifications. Good luck with your implementation!







