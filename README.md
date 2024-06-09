# DSA-notes

## Data structures 

### Arrays / ArrayList

- Good for random access and when you know the number of elements before itself
- Good for inserting elements at the end
- Each time the space gets over the ArrayList size expands to 2x leading to O(1) complexity for inserting at the end
- Bad for insertion at the start, takes O(n) time
- Bad for insertions and deletions in the middle


### LinkedList 

- Good for inserting at the start
- Good for deleting and adding in the middle
- Bad for random access

### stacks 

- LIFO ( Last in first out )
- operations
   - addFirst()
   - removeFirst()
   - first() 
- Good for adding/deleting/accessing top element
- Bad for accessing random elements

### queues 

- FIFO ( First in first out )
- operations
  - addLast()
  - removeFirst()
  - first()
  - last()
- Good for adding/deleting/getting the first and last element
- Bad for accessing random elements

### Hashmap 

- Buckets of LinkedList - this data structure is as good as the hash keys
- O(1) average-case time complexity for insertion, deletion, update, and access using a key
- O(n) worst-case time complexity for all operations.

### Binary trees 

- Non-linear data structure and a special form of a graph
- In a binary tree, Each node can have at max 2 nodes
- Traversal using BFS / DFS
- BFS
  - Level order order traversal using a queue
- DFS
  - In order ( Left root right )
    - When you traverse a binary search tree using in-order you should see elements are sorted
  - Post order ( Left right root)
  - Pre-order ( root left right ) 

### Binary search tree

- The left subtree will always be smaller than the root and the right subtree will always be greater than the root

### Self-balanced binary search tree

- In BST, there is an edge case where elements on the left or right can keep growing and lead to an O(n) search
- Self-balancing is about maintaining the tree so that the search can be O(logn) 

### Heaps 

- Always maintain the complete binary tree structure
  - Complete binary tree means when filling the tree fill from left to right
    
- Getting the min/max element will be an O(1) operation
- Insertion/deletion will be O(logn)

### Graphs 

| directed + weighted | undirected + weighted | undirected + unweighted | directed + unweighted | 
| ------------------- | --------------------- | ----------------------- | --------------------- |
| Flight tickets      | Road network          | Facebook friends        | Twitter followers, dependencies  |


## Algorithms 

### Two pointer 

### Sliding window 

### Fast & slow pointer

### In-place Reversal of linkedlist && inverting binary tree

### Modified binary search 

### BFS 

### DFS 

### Topological sort 

### Islands ( Matrix traversal ) 

### Intervals 

### Top k elements 

### K way merge 

### Cyclic sort
