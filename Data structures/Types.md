#fundamentals #data-structures 

What types of data structures are there?
?
- Arrays
- Linked Lists
- Stacks
- Queues
- Trees
- Graphs
- Hash tables
- Heaps

What are the properties of arrays?
?
- A collection of elements stored in contiguous memory locations.
- Access time for elements is constant (O(1)).
- Insertion and deletion may require shifting elements, making it O(n).
- If the array is sorted, binary search can be applied to efficiently find the occurrence of an element. Binary search has a time complexity of O(log n), making it faster than linear search. In other words, arrays are suitable when the collection is sorted because binary search can be employed, cutting down the search space logarithmically.

What are the properties of linked lists?
?
- A collection of nodes, where each node contains data and a reference to the next node.
- Efficient for insertions and deletions (O(1)).
- Access time is O(n) since it requires traversing the list.
- Linked lists are particularly efficient for insertions and deletions at any position in the list. They provide constant-time (O(1)) complexity for these operations as they involve updating references.

What are the properties of a stack?
?
- A collection of elements with last-in, first-out (LIFO) access.
- Operations include push (add to the top) and pop (remove from the top).
- Can be implemented using arrays or linked lists.

What are the properties of a queue?
?
- A collection of elements with first-in, first-out (FIFO) access.
- Operations include enqueue (add to the rear) and dequeue (remove from the front).
- Can be implemented using arrays or linked lists.

What are the properties of a tree?
?
- Hierarchical data structure with a root node and subtrees of children nodes.
- Examples include binary trees, AVL trees, and B-trees.

What are the properties of a graph?
?
- A set of nodes connected by edges, representing relationships.
- Directed and undirected graphs with various traversal algorithms (e.g., depth-first search, breadth-first search).

What are the properties of a hash table?
?
- A data structure that maps keys to values using a hash function.
- Provides constant-time average complexity for insertion, deletion, and retrieval.
- Hash tables provide constant-time average complexity for searching, making them efficient for finding elements. However, they may have collision resolution strategies that impact worst-case performance. In other words, hash tables are effective for unsorted collections as they offer constant-time average complexity for search operations. However, they rely on a good hash function and may exhibit worst-case scenarios depending on collisions.

What are the properties of a heap?
?
- A binary tree-based data structure where the key of each node is either always greater than or always less than its children.
- Used in priority queues and heap sort algorithms.
- Heaps, particularly binary heaps, are useful for maintaining a dynamically changing collection where the minimum or maximum element needs to be quickly accessed or removed. Heap operations, including insertion and deletion, have logarithmic time complexity (O(log n)).

What are dynamic arrays?
?
Dynamic arrays allow for dynamic resizing, making them suitable for efficient insertions and deletions at the end of the array. While appending to the end has amortized constant time (O(1)), inserting or deleting elements at arbitrary positions might require shifting elements, resulting in linear time (O(n)).

What are segment trees?
?
A segment tree is a binary tree where each leaf node represents an array element, and each non-leaf node represents a segment of the array. It is designed for efficient range query operations such as finding the sum, minimum, or maximum over a given range.

What are Fenwick trees?
?
A Fenwick tree is a specialized data structure for efficiently performing range queries on an array, especially when the operations are associative (like sum or min/max).

What are Graphs?
?
Graphs are a fundamental data structure for representing relationships between nodes. They can be implemented using an adjacency matrix or an adjacency list.

What are priority queues?
?
Priority queues are often used in conjunction with graph traversal algorithms, especially for weighted graphs. The priority queue helps in selecting the next node with the highest or lowest priority.