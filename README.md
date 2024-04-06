You can start playing the game using the file name "Final"

It is a simple 5X5 grid maze game which allows the user to navigate through the space one grid to another using the arrows keys 

The purpose of the game:

Navigate from the initial possition to the top right corner of the space without touching the 'Y' while touching at least a minimum of 10 'X' to Win the game

note - The game will be terminated if you touch X more than once or if you touch any Y

To ensure smooth functionining of the game ensure ti install the 'random' and 'keyboard' module in you computer

The logic behind th generated grids with at least 1 possible win scenario is the following:

1. Random Walk with Backtracking: Start from the initial position and make random moves while keeping track of the path length and ensuring we're always able to reach the goal. If the path gets too long without reaching the goal, backtrack.
2. Exact 'X' Count: Since the path must contain exactly 10 'X's, we'll need to monitor the count of 'X's in our path. If we reach the goal before having exactly 10 'X's, we'll need to intelligently add more steps without violating the other rules.
3. Ensuring Valid Moves: At each step, ensure the move is valid (stays within grid bounds and adheres to the move rules).