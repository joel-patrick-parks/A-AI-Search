Joel Parks
jpp63
Homework 1
4/28/2017

The program was tested and run on tux. The instructions will outline how to run the program on tux.

I was having a problem on tux that I was not having locally in visual studios. The OPEN and CLOSED lists, as well as the nodes, length, and time variables were not being cleared after each algorithm was run. To fix this, I'm including 4 folders, two runnning the custom heuristic on each level, and two running the manhattan heuristic on each level. The files included section will tell you which folders run which algorithm/level combinations.

COMPILATION AND EXECUTION INSTRUCTIONS
To compile the program, move all of the files within the submitted zip into the same folder on tux. Once there, navigate to the folder that the files are located in and run the command make. An executable called 'hw2' will be created in the same folder. To run the executable,  enter the command ./hw2>output-hw2.txt. The executable will run and the output will be sent to the text file 'output-hw2.txt'.

FILES INCLUDED
HW2P1 - This folder contains the cpp, make, executable, and level files to run the custom heuristic for level 1
HW2P2 - This folder contains the cpp, make, executable, and level files to run the manhattan heuristic for level 1
HW2P3 - This folder contains the cpp, make, executable, and level files to run the custom heuristic for level 2
HW2P4 - This folder contains the cpp, make, executable, and level files to run the manhattan heuristic for level 2

CUSTOM HEURISTIC
For my custom heuristic, I used the pythagorean theorem to calculate the distance between the location of the master brick and the final destination (the -1 block, the solution to the puzzle). To do this, I got the distance from the master block's x-coordinate to the solution block's (-1 block) x-coordinate, and the distance from the mater block's y-coordinate to the solution block's (-1 block) y-coordinate. I then squared each value, added them together, and then took the square root of them, which I returned for my heuristic.
    
    /|
 z / | y-distance   z = sqrt(x^2 + y^2), where z is the heuristic returned.
  /  |
 /___|
  x-distance