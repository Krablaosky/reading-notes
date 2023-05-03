# Data Structures and Algorithms

## 8 Common types

**Arrays**: Arrays are a collection of elements of the same data type. They can be accessed using an index and can be used to store and retrieve data quickly.


**Attributes**:

Ordered collection of elements of the same type
Elements are stored in contiguous memory locations
Can be accessed using index

**Applications**:

Used to store and manipulate a large collection of homogeneous data
Used to implement other data structures such as stacks, queues, and matrices
Used to store and retrieve data in databases and spreadsheets

**Linked Lists:** A linked list is a collection of nodes where each node contains data and a pointer to the next node. They can be used to implement stacks, queues, and other data structures.

**Attributes:**
Ordered collection of elements, each containing a value and a reference to the next element
Elements are not stored in contiguous memory locations
Can be singly-linked or doubly-linked

**Applications:**

Used for dynamic memory allocation in programming languages
Used to implement other data structures such as stacks, queues, and hash tables
Used to represent sparse matrices and graphs

**Stacks:** A stack is a data structure that stores elements in a last-in, first-out (LIFO) order. It can be implemented using arrays or linked lists.

**Attributes:**
Ordered collection of elements
Follows Last-In-First-Out (LIFO) principle
Can be implemented using arrays or linked lists

**Applications:**

Used to keep track of function calls in programming
Used to undo/redo operations in text editors and software applications
Used to evaluate expressions in compilers and interpreters

**Queues:** A queue is a data structure that stores elements in a first-in, first-out (FIFO) order. It can be implemented using arrays or linked lists.

**Attributes:**
Ordered collection of elements
Follows First-In-First-Out (FIFO) principle
Can be implemented using arrays or linked lists

**Applications:**

Used in scheduling algorithms to manage processes and tasks
Used to implement buffers and caches in computer systems
Used in network protocols to manage packets and messages

**Trees:** A tree is a collection of nodes where each node has a parent and zero or more children. They can be used to represent hierarchical data such as file systems or organization charts.

**Attributes:**
Hierarchical data structure with a root node and child nodes
Each node can have zero or more child nodes
Can be binary, balanced, or search trees

**Applications:**

Used to represent hierarchical data such as file systems and organization charts
Used to implement searching and sorting algorithms such as binary search and quicksort
Used in databases to store and retrieve data efficiently


**Graphs:** A graph is a collection of vertices (nodes) connected by edges. They can be used to represent relationships between entities such as social networks or transportation networks.

**Attributes:**

Non-linear data structure consisting of vertices and edges
Can be directed or undirected
Can be represented using adjacency matrix or adjacency list

**Applications:**

Used to model relationships between objects and entities such as social networks and transportation networks
Used to solve problems in areas such as optimization and routing
Used in artificial intelligence and machine learning to represent knowledge and decision-making processes

**Hash Tables:** A hash table is a data structure that maps keys to values using a hash function. They can be used to implement associative arrays, symbol tables, and other data structures.

**Attributes:**

Data structure that stores data in an associative array
Uses a hash function to map keys to indices in an array
Provides constant-time average-case complexity for operations such as insertion, deletion, and search

**Applications:**

Used in databases and file systems to store and retrieve data efficiently
Used in cryptography to generate and verify digital signatures
Used in compilers and interpreters to implement symbol tables and lexical analysis

**Heaps:** A heap is a binary tree that satisfies the heap property. They can be used to implement priority queues and are often used in sorting algorithms.

**Attributes:**

Binary tree-based data structure
Follows the heap property that the value of each node is greater than or equal to the values of its children (max heap) or less than or equal to the values of its children (min heap)
Can be implemented using arrays or linked lists

**Applications:**

Used to implement priority queues in algorithms and applications such as Dijkstra's algorithm and Huffman coding
Used in sorting algorithms such as heapsort and selection sort
Used in memory management algorithms such as garbage collection in programming languages

## Big O Notation

### [Cheat Sheet](https://www.bigocheatsheet.com/)

Big O notation is a way of describing the efficiency of an algorithm or the performance of a function. It helps us analyze the time complexity and space complexity of an algorithm as its input size grows. In other words, it helps us understand how the performance of an algorithm changes as we increase the size of the input.

The notation is expressed as O(f(n)), where f(n) represents the upper bound of the algorithm's time complexity in terms of the input size n. The "O" stands for "order of" and represents the worst-case scenario for the algorithm's time complexity.

There are several common notations used in Big O analysis, including:

O(1): This notation represents constant time complexity, meaning that the algorithm's performance does not depend on the input size. This is the most efficient time complexity and is often the goal of optimization efforts.
Example: Accessing an element in an array by index.

O(log n): This notation represents logarithmic time complexity, meaning that the algorithm's performance increases logarithmically as the input size grows. This is more efficient than linear time complexity.
Example: Binary search algorithm.

O(n): This notation represents linear time complexity, meaning that the algorithm's performance grows linearly with the input size. This is the most common time complexity and is often considered acceptable.
Example: Traversing an array or linked list.

O(n log n): This notation represents n log n time complexity, which is between linear and quadratic. It is often seen in sorting algorithms.
Example: Merge sort algorithm.

O(n^2): This notation represents quadratic time complexity, meaning that the algorithm's performance grows exponentially with the input size. This is less efficient than linear time complexity.
Example: Bubble sort algorithm.

O(2^n): This notation represents exponential time complexity, meaning that the algorithm's performance doubles with each increase in the input size. This is extremely inefficient and should be avoided if possible.
Example: Recursive Fibonacci sequence algorithm.

It's important to note that Big O notation only represents the upper bound of an algorithm's time complexity. It doesn't take into account best-case or average-case scenarios, and it doesn't account for the constant factors that affect an algorithm's performance.

Big O notation is a way of analyzing the time complexity and space complexity of an algorithm as its input size grows. By understanding the notation and its common notations, we can analyze and optimize our algorithms to improve their performance.

## Discussion Questions

1. What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?

* When deciding which data structure is best suited to solve a particular problem, one of the more important things to consider is the efficiency of the data structure for the specific task at hand. This involves considering factors such as the time complexity and space complexity of the data structure, as well as the expected size and type of data that will be processed. For example, if the task involves searching or sorting large amounts of data, a data structure with fast search or sort times, such as a hash table or a balanced binary search tree, may be a good choice. On the other hand, if the task involves maintaining a collection of items in a particular order, a linked list or an array may be more suitable.

2. How can we ensure that we’ll avoid an infinite recursive call stack?

* To avoid an infinite recursive call stack, it is important to ensure that recursive functions have a base case that will terminate the recursion. The base case defines the simplest possible case that can be solved without recursion. When the base case is reached, the recursion stops and the function returns a result. For example, in a recursive function that computes the factorial of a number, the base case would be when the number is 1, as the factorial of 1 is 1. When the recursive function encounters this base case, it returns the value 1, and the recursion stops. Additionally, it is important to ensure that the recursion depth is limited to a reasonable number. This can be achieved by carefully designing the recursive algorithm to ensure that the maximum recursion depth is proportional to the size of the input data.