Welcome to the BlackHole wiki!

This page describes the usage of "BlackHole" algorithm implementation.

**Environment Setting**

- The results can be guaranteed with linux 64-bit environment. If you use 32-bit environment, you should install linux-64 bit before. 

**Installation & Running**

- Download the BlackHole file in github.
  * wget https://github.com/kujungmul/BlackHole/archive/master.zip

- Follow these commands
  * unzip master.zip
  * cd BlackHole-master/Debug

- Compile source codes
  * make clean
  * make all

- Run the program
  * ./BlackHole [Input Edge List FILE] [DIMENSION] [Alpha] [MinPTS] [Pruning Rate]
  * example) ./BlackHole ../Data/football.dat 2 0.05 5 0.1

**File & Directory Structure**
- Debug : including make file
- Data : football, synthetic network data & output data
- src : source code and header file

**Output Data**
- [Input Edge List FILE]_position.out : Index / X / Y : each row means index, x, and y position. there is no clustering information
- [Input Edge List FILE]_position.out_MinPts [MinPTS]_RemovePrecent [PruningRate]_EPS [EstimationParam].dat : Index / clusterID / core : this file include each node's cluster information

If you have any question, feel free to email me. (kujungmul@gmail.com)
