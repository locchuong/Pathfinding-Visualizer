# Pathfinding Visualizer
A simple pathfinding visualizer built on react. I made this app while learning to work with react so I may have commited some react crimes, but hopefully someone will provide some insight on this; I'm open to criticism. If you'd like to try this web app out, feel free to access it [here](https://pathfinding-visualizer-react.herokuapp.com/). Additionally, feel free to fork this if you'd like to base your projects off this, I had a lot of fun creating this project. A special thanks to Clement Mihailescu for his youtube tutorial which introducted me to working with react.

## Algorithms
**Dijkstra's Algorithm**: Developed by Edsger W. DIjkstra, this algorithm guarantees the shortest path between two nodes in a graph. It does so by repeatedly expanding the closest vertex which has not been visited in conjunction with a priority queue of distance values from the start node. Note that this algorithm is weighted.

**Breath-first Search**: This algorithm guarantees the shortest path between two nodes in a graph by exporting all neighbor nodes at the present depth prior to moving on to the next depth level of nodes. It does so using a queue as its data structure. Note that this algorithm is unweighted.

**Depth-first Search**: This algorithm does **not** guarantee a shortest path and is a terrible algorithm for pathfinding. DFS explores as far as possible along each "branch" before backtracking. While it does guarantee a path to the end node, it is almost always not the shortest path.

**A STAR Search Algorithm**: This algorithm is a graph traversal and path finding algorithm that guarantees the shortest path using heuristics to guide it. It does so by keeping track of a fcost, hcost and gcost where hcost is the projected distance from any given node to the end node and gcost is the distance to the start node. Fcost is simply hcost + gcost. The heuristic used in this implementation is Euclidean distance, but Manhattan distance is also implemented (commented out). The data structure used to implement this algorithm was a priority queue which orders the nodes by fcost.

**Recursive Subdivision**: This algorithm picks a random pivot point, creates a wall at the pivot with a random passages along it, and then recursively calls the algorithm on the subdivided regions. Because entire cells (Instead of the outline of the cells) were used as walls, walls are restricted to having even-numbered indices and passages are restricted to odd-numbered indices.
