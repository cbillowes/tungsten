#algorithms

What is topological sorting?
?
- Topological sorting is a linear ordering of the vertices in a directed acyclic graph (DAG) such that for every directed edge (`u`,`v`), vertex `u` comes before `v` in the ordering, providing a consistent sequence that respects the partial order defined by the edges in the graph.
- It is like arranging tasks in a to-do list where each task depends on the completion of others; the goal is to order the tasks so that you can follow the list and never encounter a task before its dependencies are done. In a graph, tasks are represented as vertices, and dependencies are shown as directed edges between them, creating a directed acyclic graph (DAG). 
- Topological sorting ensures that you process the vertices in an order that respects these dependencies, preventing you from encountering a task before its prerequisites are completed.

What is a directed acyclic graph (DAG)?
?
- A directed acyclic graph (DAG) is a graph structure that consists of vertices (nodes) connected by directed edges, where each edge has a specific direction indicating a one-way relationship between nodes. 
- Importantly, a DAG does not contain any cycles, meaning there is no sequence of directed edges that loops back to a starting vertex. This acyclic property makes DAGs useful in modeling scenarios where certain tasks or events must occur in a specific order without creating circular dependencies.

What are commonly used algorithms used with Directed Acyclic Graphs (DAGs)?
?
1. **Topological Sorting:**
	Determines a linear ordering of vertices in a DAG such that for every directed edge (u, v), vertex u comes before v in the ordering.
1. **Shortest Path Algorithms:**
	Algorithms like Dijkstra's and Bellman-Ford are used to find the shortest paths between vertices in a DAG, considering the direction of edges.
1. **Critical Path Analysis:**
    Identifies the critical path in a DAG, which represents the longest path through the graph and determines the minimum time needed to complete a project.
2. **Dynamic Programming:**
    DAGs are often used in dynamic programming to optimize recursive algorithms by memoizing intermediate results in a topological order.
3. **Minimum Spanning Tree (MST):**
    Algorithms like Kruskal's and Prim's can find the minimum spanning tree in a weighted DAG, representing the subset of edges that connect all vertices with minimum total weight.
4. **Flow Networks and Maximum Flow:**
    DAGs can be used to model flow networks, and algorithms like Ford-Fulkerson can find the maximum flow in such networks.
5. **Dependency Resolution:**
    DAGs are commonly employed in build systems and task scheduling to resolve dependencies and determine the order in which tasks or modules should be executed.
6. **Pattern Matching and Recognition:**
    DAGs can represent patterns in various applications, and algorithms can be designed to efficiently match or recognize these patterns.

