#theory 

Studies structures made of **vertices (nodes)** and **edges (connections)**.

- A **graph** is defined as \( G = (V, E) \), where:
  - \( V \) = set of vertices.
  - \( E \) = set of edges (pairs of vertices).

---
### Types of Graphs

- **Undirected Graph:** Edges have no direction.
- **Directed Graph (Digraph):** Edges have a direction (arrows).
- **Weighted Graph:** Each edge has a weight or cost.
- **Simple Graph:** No loops or multiple edges.
- **Multigraph:** Allows multiple edges between two vertices.
- **Complete Graph \( K_n \):** Every pair of distinct vertices is connected.
- **Bipartite Graph:** Vertices can be split into two sets, with edges only between sets.
- **Tree:** A connected graph with no cycles.

---
### Basic Terminology

- **Degree (deg(v)):** Number of edges incident to vertex \( v \).
- **Path:** A sequence of edges connecting a sequence of vertices.
- **Cycle:** A path that starts and ends at the same vertex, with no repetition of edges or vertices (except the start/end).
- **Connected Graph:** There is a path between every pair of vertices.
- **Component:** A maximal connected subgraph.
- **Adjacency:** Two vertices are adjacent if they share an edge.
- **Adjacency Matrix:** \( A[i][j] = 1 \) if \( i \) and \( j \) are connected, else 0.
- **Adjacency List:** List of neighbors for each vertex.

---
### Important Properties

- **Eulerian Path/Circuit:**  
  - A path or circuit that visits every edge exactly once.
  - A graph has an Eulerian circuit iff every vertex has an even degree.
- **Hamiltonian Path/Cycle:**  
  - A path or cycle that visits every vertex exactly once.
  - No simple characterization like Eulerian paths.

---
### Common Algorithms

- **DFS (Depth-First Search):** Explore as deep as possible before backtracking.
- **BFS (Breadth-First Search):** Explore all neighbors first (layer by layer).
- **Dijkstra’s Algorithm:** Shortest path for weighted graphs (non-negative weights).
- **Bellman-Ford Algorithm:** Shortest path with possible negative weights.
- **Floyd-Warshall:** All-pairs shortest path.
- **Kruskal’s Algorithm:** Minimum Spanning Tree (MST) using edge sorting.
- **Prim’s Algorithm:** MST starting from a vertex.

---
### Applications

- Network routing (internet, social networks).
- Scheduling problems.
- Circuit design.
- Pathfinding in maps.
- Modeling relationships (e.g., bipartite matching).