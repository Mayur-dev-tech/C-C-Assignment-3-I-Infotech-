River Crossing Puzzle Simulation

This program simulates a river crossing puzzle where a boatman needs to transport entities (Sheep, Lion, Grass) across a river while adhering to certain rules to avoid conflicts.

Instructions:

1. Compilation:

Ensure you have a C++ compiler installed on your system (e.g., g++ for Linux, MinGW for Windows).
Open a terminal or command prompt.
Navigate to the directory containing the source code files.
Compile the code using the following command:

[g++ -std=c++11 -o river_crossing river_crossing.cpp]

2. Execution:

After successful compilation, run the executable file using the following command:
[./river_crossing]
The program will start, displaying a menu with options to transport Sheep, Lion, or Grass across the river.
Enter the corresponding number for your choice and press Enter.
Follow the instructions displayed on the screen to continue transporting entities until the puzzle is solved or you choose to exit.



Explanation of Design Choices:

Global Vectors: currentSide and goalSide are used to represent the entities currently on each side of the river. They are declared globally for ease of access across different functions.
Mutex: A mutex (mtx) is used to ensure thread safety when accessing shared resources such as the log file and the global vectors.
Error Handling: Exceptions are thrown and caught to handle errors encountered during the boatman's actions or program execution.
Log File: A log file (river_crossing_log.txt) is created to log the boatman's actions and any errors encountered during the program execution.
Menu Interface: A simple menu interface is provided for user interaction, allowing them to choose which entity to transport across the river.
Overall, the code provides a basic simulation of a river crossing puzzle, demonstrating the use of multithreading, synchronization, error handling, and logging in a C++ application.
