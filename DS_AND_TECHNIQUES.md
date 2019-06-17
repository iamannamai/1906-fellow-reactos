# Data Structures and Common Techniques

## Linked Lists

- "Runner" Technique - pointers moving at different speeds
- Recursion common in linked list problems

## Stacks

- Recursive problems may use stacks to store data (push and then pop on the way out)
- Stacks can be used to implement recursive solutions iteratively

## Queues

- Breadth-first searches
- Implementing caches

## Tree

- A tree is just another graph!
- Typically recursive
- "Balancing" a tree typically refers to "balancing a tree enough" to ensure that inserts and finds are `O(log n)`. If interested, look into `Red-Black` and `AVL` trees in CtCI (advanced topics).

## Binary Tree Traversal

- in-order (left, current, right) - ascending order
- post-order (current, left, right) - visits root first
- pre-order (left, right, current) - root is always last

## Binary Heaps (Min)

- complete binary trees, each node smaller than its children, root is smallest
- `insert` - `O(log n)`, bubble up
- `extractMin` - `O(log n)`, replace root with last child, bubble down
- use an array

## Graphs

- Nodes/Vertices and Edges (directed edges go one way, undirected go in both directions)
- Adjacency Lists - every vertex stores a list of adjacent vertices. Can represent as:
  - hash table where each node is a key that stores an array of adjacent nodes
  - `Graph` class where every `Node` stores a list of adjacent nodes
- Adjacency Matrices - NxN boolean matrices
  - symmetric for undirected graphs
- Search graphs using `BFS` or `DFS`
  - Depth-First
    - explore each branch completely before moving on to next branch
    - preferred if need to visit every node in branch
    - must check if a node has been visited
  - Breadth-First
    - explore each neighbor before going on to any of their children
    - finding shortest/any path between nodes
    - use a queue!
  - Bidirectional Search - run simultaneous BFSs starting from both the source and the target (as opposed to just doing a BFS from source until you find target) - searches will collide after d/2 levels
