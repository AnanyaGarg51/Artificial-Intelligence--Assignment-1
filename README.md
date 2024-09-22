# Artificial-Intelligence--Assignment-1

This Github repository is my submission for the first programming assignment of the Artificial Intelligence course. Here I have solved the classis BOAT Problem using 3 search algorithms- BFS, DFS, and DFID. I could not complete solving the eight-puzzle problem due to time constraints, but willl surely submit it for review and correction as sson as possible. In this Reaadme file I explain my approach in detail:
<br>
<br>
<h2>REPRESENTATION OF THE PROBLEM AS A SEARCH SPACE</h2>
<br>
In this implementation, the state of the problem is represented as a TUPLE.
The first element is a set containing the entities (Lion, Goat, Cabbage) on the left bank of the river.
The second element is a string that indicates the current position of the boat: either 'LEFT' or 'RIGHT'.
Each state corresponds to a unique configuration of where the farmer, lion, goat, and cabbage are in relation to the riverbanks. The goal is to move all entities from the left bank to the right bank without violating the constraints (lion cannot be left with goat, goat cannot be left with cabbage without supervision).
<br>
<br>
<h2>SEARCH ALGORITHMS USED:</h2>
<br>
<h4>Breadth-First Search (BFS)</h4>
BFS explores the search space level by level, starting from the initial state and expanding all possible moves before going deeper. It ensures that the shortest path is found but can consume a lot of memory as it stores all nodes at each level.
<br>
<br>
<h4>Depth-First Search (DFS)</h4>
DFS explores one path fully before backtracking to try other possibilities. It uses less memory than BFS because it doesn’t store all nodes at the current depth, but it may not find the shortest solution and can get stuck in deep paths.
<br>
<br>
<h4>Depth-First Iterative Deepening (DFID)</h4>
DFID combines the benefits of BFS and DFS. It performs DFS but with increasing depth limits, ensuring that it finds the shortest path while using less memory than BFS. It explores nodes gradually deeper with each iteration, making it both space-efficient and complete.
<br>
<br>
<br>
<h2>SPACE AND TIME COMPLEXITY ANALYSIS</h2>
TIME COMPLEXITY is analogous to NUMBER OF NODES EXPLORED
<br>
BFS= 19
DFS= 10
DFID= 34
This clearly demonstrates that while the time complexity of BFS and DFS is nearly comparable, DFID takes a considerably greater time than both BFS and DFS.
<br>
<br>
SPACE COMPLEXITY is analogous to SIZE OF OPEN QUEUE
<br>
BFS= 6
DFS= 8
Clearly, DFID is better on the space comlexity part compared to BFS, thus acting as an optimization between DFS and BFS.
