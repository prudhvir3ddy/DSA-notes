# DSA-notes

## Coding interview lessons

- Remember and learn patterns, not code

- Convert 1-liners to code: When looking at a solution, don't read it completely. Just read a line and go back to the problem and struggle again (Interviewers will give the hints and this ability to go back and struggle will help you there )

- Communicate a lot during the interview, one problem and two brains is much better, so you don't have to waste time explaining the solution

- Trust the process blindly, you will get better at coding

![Screenshot 2024-06-23 at 8 56 41 AM](https://github.com/prudhvir3ddy/DSA-notes/assets/20471162/fc5df1cf-a851-4081-b318-165abe69d5c7)

source of those lessons: https://www.youtube.com/playlist?list=PL7NYbSE8uaBDEXmgcdfyqY7sJ9wkf4W7q 

### Under 35 mins 

 1. Listen & understand the question
 2. Think of edge cases
 3. Brute force solution
 4. Optimising
 5. Walk through your approach
 6. Implement
 7. Test and dry run
 8. Finish questions quickly, So they can ask follow-up questions

### Best strategy for getting better at coding 

Solve x problems per day and do it every single day till your dream offer

x - amount of healthy time you can give after your working hours, chores and workout

You can go through world class content but if you don't do this, you will always feel stuck

If you solve questions every day 

Most things stay in your memory cache head, For example, you don't have to think about how to generate subarrays, how to do BFS/DFS

In interviews,

Generating subarrays or BFS/DFS will be just a part of the problem. If you spend a lot of time trying to figure out how to do this like normal brain 

you will be out of time to solve the actual question

Most interview problems are medium-level questions 

Medium-level questions usually are a combination of 2+ easy questions. 

For the average brain which didn't practice medium-level questions, even with all the hints it will take 45+ minutes 

### For a brain which is solving questions every day 

- Can focus on the actual complicated part of the problem instead of worrying about silly things 
- improved coding speed
- hints interviewers give you are limited so why not let him good hints that matter and not the hints of silly coding mistakes
- less debugging
- opens the scope to write clean code in interviews
  
![Screenshot 2024-06-23 at 9 01 59 AM](https://github.com/prudhvir3ddy/DSA-notes/assets/20471162/6c93756c-c535-4da4-86e8-c7c1265acfee)

### An edge case in preparation strategy

While you are solving problems, for many problems you will either have to look at the solution or look at the hints or you will make major coding errors

Note down those problems and repeat solving the same problem again after x days

There are high chance that if you face the same problem again, you won't be able to come up with a solution on your own if you watched the solution

Solve those questions repeatedly with a few days break in the middle and you will grasp that concept.

### A few points for coding interviews

Write code only after figuring out the problem in and out 

If you start coding without solving the problem, you won't be able to write code

This is a common problem for most, why? 

1. Writing boilerplate code makes us feel like we are making progress --> no it's not
2. So that we don't forget what we solved already --> write notes in English for that and not code or even pseudo code if it's a complicated logic
3. During development, we got used to intellisense of repeated work we do  --> coding interview is a new problem and the problem will change in the middle

Starting code without solving the problem will waste a lot of time not knowing what to write
Coding will be the easiest part in the 45 min round and give it only 5-10 minutes

Because there are limited things to remember and most of it is in your memory cache by practice you should be comfortable with most coding

if you know what to write you should be able to write 

whether it's recursion, backtracking, two pointers, BFS/DFS, binary search 

During the interview, you shouldn't be thinking 

whether binary search logic is 

low < high or 
low <= high 

you should know it already. 

You will not think while writing loops, other standard algorithms should also stick in your brain that way to increase your chances  

### Resources for learning 

There are 100s of resources, use the DFS approach here

Just pick 2-3 resources and go in-depth instead if you try many resources you will cover basics in all which is not useful. 

- techinterviewhandbook.org
- leetcode.com
- neetcode.io/roadmap
- bigocheatsheet.com

Important LC links
https://leetcode.com/discuss/general-discussion/665604/Important-and-Useful-links-from-all-over-the-LeetCode/

Linked List - https://leetcode.com/discuss/study-guide/1800120/become-master-in-linked-list

Tree traversals - https://leetcode.com/discuss/study-guide/937307/Iterative-or-Recursive-or-DFS-and-BFS-Tree-Traversal-or-In-Pre-Post-and-LevelOrder-or-Views

Recursion - https://leetcode.com/discuss/study-guide/1733447/become-master-in-recursion

Backtracking - https://leetcode.com/problems/permutations/solutions/18239/A-general-approach-to-backtracking-questions-in-Java-(Subsets-Permutations-Combination-Sum-Palindrome-Partioning)/

substring - https://leetcode.com/problems/minimum-window-substring/solutions/26808/Here-is-a-10-line-template-that-can-solve-most-'substring'-problems/

Sliding window - https://leetcode.com/problems/frequency-of-the-most-frequent-element/solutions/1175088/C++-Maximum-Sliding-Window-Cheatsheet-Template/

Two pointer - https://leetcode.com/discuss/study-guide/1688903/Solved-all-two-pointers-problems-in-100-days

Binary search - https://leetcode.com/discuss/study-guide/786126/Python-Powerful-Ultimate-Binary-Search-Template.-Solved-many-problems

Monotonic stack - https://leetcode.com/discuss/study-guide/2347639/A-comprehensive-guide-and-template-for-monotonic-stack-based-problems

Graphs - https://leetcode.com/discuss/study-guide/655708/Graph-For-Beginners-Problems-or-Pattern-or-Sample-Solutions

DP - https://leetcode.com/discuss/study-guide/458695/Dynamic-Programming-Patterns

## Data structures 

### Arrays / ArrayList

- Good for random access and when you know the number of elements before itself
- Good for inserting elements at the end
- Each time the space gets over the ArrayList size expands to 2x leading to O(1) complexity for inserting at the end
- Bad for insertion at the start, takes O(n) time
- Bad for insertions and deletions in the middle

```kotlin
val array = Array(5) {
//If you want to initialise the array with a default value
    0
}

array[1] = 1

val array2 = arrayOf(1,2,3)

val arrayList = arrayListOf<String>()

arrayList.add("Hello")

```

#### common concepts

- subarrays, subsequences, subsets
- Longest substring without repeating charaters
  - use the data structure which remembers what we seen before
  - update the first pointer till there are no duplicates 
- Maximum subarray
  - Trick is make sure to calculate the running sum
  - Check if it's worth to add up negative numbers 

### LinkedList 

- Good for inserting at the start
- Good for deleting and adding in the middle
- Bad for random access

```kotlin
data class Node(
    var data: Int,
    var next: Node? = null,
    var prev: Node? = null, // for doubly linked list
)
```

#### common questions 

- Reversing the LinkedList
  - try to reverse one link and repeat
- questions based on the fast-slow pointer technique
- starting point of cycle in the LinkedList

### stacks 

- LIFO ( Last in first out )
- operations
   - addFirst()
   - removeFirst()
   - first() 
- Good for adding/deleting/accessing top element
- Bad for accessing random elements

#### common questions 

- valid brackets

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
- Use it to remember the past 

### Binary trees 

- Non-linear data structure and a special form of a graph
- In a binary tree, Each node can have at max 2 nodes

 
#### common questions 

- inverting a binary tree
- diameter of a binary tree
- the height/depth of a binary tree
- Traversal using BFS / DFS
- BFS
  - Level order order traversal using a queue
- DFS
  - In order ( Left root right )
    - When you traverse a binary search tree using in-order you should see elements are sorted
  - Post order ( Left right root)
  - Pre-order ( root left right )
- Print path from root to any node
- Least common ancestor

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
