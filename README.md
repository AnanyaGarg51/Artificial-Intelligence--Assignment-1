# Artificial-Intelligence--Assignment-1

This Github repository is my submission for the first programming assignment of the Artificial Intelligence course. Here I have solved the classis BOAT Problem using 3 search algorithms- BFS, DFS, and DFID. I could not complete solving the eight-puzzle problem due to time constraints, but willl surely submit it for review and correction as sson as possible. In this Reaadme file I explain my approach in detail:
<br>
REPRESENTATION OF THE PROBLEM AS A SEARCH SPACE
<br>
In this implementation, the state of the problem is represented as a TUPLE.
The first element is a set containing the entities (Lion, Goat, Cabbage) on the left bank of the river.
The second element is a string that indicates the current position of the boat: either 'LEFT' or 'RIGHT'.
Each state corresponds to a unique configuration of where the farmer, lion, goat, and cabbage are in relation to the riverbanks. The goal is to move all entities from the left bank to the right bank without violating the constraints (lion cannot be left with goat, goat cannot be left with cabbage without supervision).
