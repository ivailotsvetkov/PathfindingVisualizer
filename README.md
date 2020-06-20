# PathfindingVisualizer

<i>Welcome to Pathfinding Visualizer! I built this application because I was fascinated by pathfinding algorithms, and I wanted to visualize them in action. I hope that you enjoy playing around with this visualization tool just as much as I enjoyed building it.
Have a look at what I am proud to present (use Goolge Chrome!) :</i>
https://ivailotsvetkov.github.io/PathfindingVisualizer/

<h1>Meet the Algorithms</h1>
This application supports the following algorithms:

<b>Dijkstra's Algorithm (weighted):</b> the father of pathfinding algorithms; guarantees the shortest path

<b>A Search* (weighted):</b> arguably the best pathfinding algorithm; uses heuristics to guarantee the shortest path much faster than Dijkstra's Algorithm

<b>Greedy Best-first Search (weighted):</b>  a faster, more heuristic-heavy version of A*; does not guarantee the shortest path

<b>Swarm Algorithm (weighted):</b>  a mixture of Dijkstra's Algorithm and A*; does not guarantee the shortest-path

<b>Convergent Swarm Algorithm (weighted):</b>  the faster, more heuristic-heavy version of Swarm; does not guarantee the shortest path

<b>Bidirectional Swarm Algorithm (weighted):</b>  Swarm from both sides; does not guarantee the shortest path

<b>Breath-first Search (unweighted):</b>  a great algorithm; guarantees the shortest path

<b>Depth-first Search (unweighted):</b>  a very bad algorithm for pathfinding; does not guarantee the shortest path

<em>On top of the pathfinding algorithms listed above, I implemented a Recursive Division Maze Generation algorithm.</em>

More about the Swarm Algorithm
The Swarm Algorithm is an algorithm that I - at least presumably so (I was unable to find anything close to it online) - co-developed with a good friend and colleague, Hussein Farah. The algorithm is essentially a mixture of Dijkstra's Algorithm and A* Search; more precisely, while it converges to the target node like A* , it still explores quite a few neighboring nodes surrounding the start node like Dijkstra's. The algorithm differentiates itself from A* through its use of heuristics: it continually updates nodes' distance from the start node while taking into account their estimated distance from the target node. This effectively "balances" the difference in total distance between nodes closer to the start node and nodes closer to the target node, which results in the triangle-like shape of the Swarm Algorithm. We named the algorithm "Swarm" because one of its potential applications could be seen in a video-game where a character must keep track of a boss with high priority (the target node), all the while keeping tracking of neighboring enemies that might be swarming nearby.
