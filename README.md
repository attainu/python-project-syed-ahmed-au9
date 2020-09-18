Maze Solver:

The aim of this project is to build a python program that runs as a command-line tool. It should take the input and output file name as command-line arguments. Using the square matrix present in the input file it should generate a path to reach the end of the maze and put it in the output file. If the maze is unsolvable, it should return -1 as the only value in the output file. 

Following are the import we use in this project:--
1. Defaultdict
2. Sys
3. Argparse

maze.py:
 We make graph
 add edge u & v
 determined if the graph is connected
 Dijxtra algorithm to find the shortest path 
 used function to find the path between source point to destination point
 add argument for input, output and source and dest point.
 

Some Sample Code

Input file contains data like this:

5
1 1 1 1 1
1 0 0 0 1
1 0 0 0 1
1 0 0 1 1
1 1 1 0 1

Where 0 is all the blocked paths and 1 is all the paths that you can go to. Now the task is to go through any 1 possible path and give it in the output file. We have to mark all the points you have visited while traversing the path as 1. So, the output file will contain:

1 1 1 1 1
0 0 0 0 1
0 0 0 0 1
0 0 0 0 1
0 0 0 0 1




