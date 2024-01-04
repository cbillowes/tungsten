#fundamentals  #data-structures

What are the trade-offs of choosing a data structure?
?
- Different data structures have trade-offs in terms of time and space complexity.
- Choosing the right structure depends on the specific requirements of the problem at hand.

What considerations do you need to take into account when choosing a data structure?
?
- Understand the access patterns, insertion/deletion frequencies, and the size of the dataset.
- Consider the operations that need to be performed efficiently.

What data structure would be a good fit for finding the occurrence of a specific element in a collection?
?
- **Arrays** are suitable when the collection is sorted because binary search can be employed, cutting down the search space logarithmically.
    
- **Hash tables** are effective for unsorted collections as they offer constant-time average complexity for search operations. However, they rely on a good hash function and may exhibit worst-case scenarios depending on collisions.

What data structures could you use to maintain a dynamic collection with efficient insertions and deletions?
?
- **Linked lists** excel at insertions and deletions because they don't require shifting elements around. However, random access is slower compared to arrays.
    
- **Dynamic arrays**, like Python lists or Java ArrayLists, are efficient for insertions and deletions at the end, thanks to their dynamic resizing. However, operations in the middle might be less efficient due to potential element shifting.
    
- **Heaps** are suitable when the priority of elements is important, and you need quick access to the minimum or maximum element. The heap property ensures efficient insertion and deletion of the root element.

What data structures could you use to ensure uniqueness of elements in a collection?
?
- Sets, implemented as HashSet or TreeSet, are explicitly designed to ensure uniqueness. HashSet provides constant-time average complexity for essential operations, making it efficient for maintaining a unique collection. TreeSet adds the benefit of maintaining elements in sorted order.
    
- Hash tables can be used to ensure uniqueness by using the keys as unique identifiers. Checking for the existence of an element and adding or removing it can be achieved with good average-case time complexity.

What data structures can you use to maintain elements in a specific order?
?
- Arrays are suitable when the order is static or changes infrequently, as they provide fast access by index. However, dynamic changes to the order might be less efficient.
    
- Linked lists are beneficial when dynamic changes to the order are frequent since insertions and deletions can be done with constant time complexity. However, random access to elements is less efficient.
    
- Trees, such as binary search trees, are well-suited for maintaining an ordered collection with efficient insertions, deletions, and searches. AVL trees ensure balance, avoiding performance degradation in worst-case scenarios.
    
- Heaps, while maintaining order in terms of priority (min-heap or max-heap), do not provide a complete sorted order. They are efficient for finding the minimum or maximum element.

What data structures could you use to efficiently search for words with given prefix or substring?
?
- Tries are specifically designed for efficient prefix-based searches. Each level in the trie corresponds to a character in the word, and the nodes at each level are linked to form complete words. This structure enables quick searches for words with a given prefix or substring.
    
- Trie operations have a time complexity proportional to the length of the word or prefix being searched, making them efficient for tasks like autocomplete or searching for all words with a common prefix.

What data structures could you use to perform queries on a range of elements, such as finding the sum or minimum/maximum?
?
- **Segment Tree:**
    Segment trees allow for efficient range queries by dividing the array into segments and precomputing information about each segment. This allows for operations like finding the sum, minimum, or maximum over a specified range in logarithmic time.
    
- **Fenwick Tree:**
    Fenwick trees, also known as Binary Indexed Trees, are particularly useful for range queries and updates. They offer efficient prefix-based operations, making them suitable for tasks like cumulative sum queries.

What data structures could you use to traverse and search for paths in a graph?
?
- **Graphs:**
	Graphs represent a set of nodes (vertices) connected by edges. The choice between an adjacency matrix or an adjacency list depends on the characteristics of the graph (dense or sparse). Adjacency matrices are efficient for dense graphs, while adjacency lists are suitable for sparse graphs.
	
- **Priority Queue:**
    Priority queues help manage the order in which nodes are processed during graph traversal. For example, Dijkstra's algorithm for finding the shortest path and Prim's algorithm for minimum spanning trees often use priority queues to select the next node efficiently.

What data structures could you use to check if a given expression has balanced parentheses?
?
Stack

What data structures could you use to implement undo and redo functionalities?
?
Stack

What data structures could you use to optimize access to frequently used data?
?
Cache (LRU Cache), Memoization (using Hash Tables)

What data structures could you use to process tasks based on priority levels?
?
Priority Queue (Binary Heap, Fibonacci Heap)

What data structures could you use to find the shortest path between two nodes in a network?
?
Graphs (Weighted edges), Priority Queue (Dijkstra's algorithm)

What data structures could you use to manage identifiers and their associated information during compilation?
?
Symbol Table (Hash Table, Binary Search Tree)

What data structures could you use to identify occurrences of a pattern in a text?
?
Trie, Hashing

What data structures could you use to efficiently search for records in a database?
?
B-Tree, Hash Index

What data structures could you use to schedule tasks based on their priority and dependencies?
?
Directed Acyclic Graph (DAG), Topological Sorting

What data structures could you use to perform queries on spatial data (e.g., geographic coordinates)?
?
Quadtree, Octree

What data structures could you use to perform substring search, manipulation, or matching?
?
Suffix Tree, Suffix Array

What data structures could you use to retrieve data from a database based on various criteria?
?
Indexes (B-Tree, Hash Index), Hash Table

What data structures could you use to maintain and update a leaderboard in real-time?
?
Priority Queue (Heap)