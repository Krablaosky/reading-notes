# Linked List

### What is a Linked List?
A linked list is a linear data structure used to store a collection of elements. Unlike arrays, linked lists do not require contiguous memory locations. Instead, they consist of nodes, where each node contains the element and a reference (or link) to the next node in the list.

### Why use Linked Lists?
Linked lists offer several advantages:

### Dynamic Size: Linked lists can grow or shrink dynamically during program execution, as memory allocation is performed on-demand.
Insertion and Deletion: Adding or removing elements in a linked list is efficient as it involves updating the references between nodes, without the need for shifting elements like in arrays.
Memory Utilization: Linked lists utilize memory efficiently by allocating memory for each element individually.
How does a Linked List work?
A linked list is made up of nodes. Each node contains two components:

### Data: The actual value or element stored in the node.
Next: A reference or link to the next node in the list.
The first node in the list is called the head, and the last node points to null, indicating the end of the list.

### Example:
Let's consider an example of a linked list that stores integer values: 4 -> 7 -> 2 -> 9 -> null.

### Diagram:

```
4 -> 7 -> 2 -> 9 -> null
```

In this example, the head node contains the value 4, and it has a reference to the next node containing 7. Similarly, the node with the value 7 has a reference to the node with the value 2, and so on, until the last node with the value 9, which points to null, indicating the end of the list.

By following the references from the head node, we can traverse the linked list and access or modify its elements.

### Conclusion:
Linked lists are versatile data structures that provide dynamic size and efficient insertion/deletion operations. Understanding the structure and properties of linked lists is crucial for effectively implementing and utilizing them in programming.


## Linked List Cheat Sheet:

Definition:

A linked list is a linear data structure where elements are stored in nodes.
Each node contains data and a reference (link) to the next node in the list.
The last node points to null, indicating the end of the list.
Types of Linked Lists:

Singly Linked List: Each node has a reference to the next node.
Doubly Linked List: Each node has references to both the previous and next nodes.
Circular Linked List: The last node points back to the first node, creating a circular structure.
Basic Operations:

Insertion:

Adding a new node to the linked list.
Can be done at the beginning, end, or any position in the list.
Deletion:

Removing a node from the linked list.
Can be done from the beginning, end, or any position in the list.
Traversal:

Visiting each node in the list sequentially.
Starts from the head node and follows the links until the end of the list.
Searching:

Finding a specific value in the linked list.
Requires traversing the list and comparing each node's data.
Advantages of Linked Lists:

Dynamic Size: Linked lists can grow or shrink during runtime.
Efficient Insertion and Deletion: Adding or removing elements is faster compared to arrays.
Memory Utilization: Linked lists allocate memory as needed, avoiding wasted space.
Disadvantages of Linked Lists:

No Random Access: Accessing a specific element requires traversing the list from the beginning.
Extra Memory Overhead: Each node requires additional memory to store the reference to the next node.
Time Complexity:

Access: O(n) - Must traverse the list from the beginning to access an element.
Search: O(n) - In the worst case, all nodes need to be examined.
Insertion: O(1) - If performed at the beginning or with a reference to the insertion point.
Deletion: O(1) - If performed at the beginning or with a reference to the deletion point.

## [Back](../401readingNotes.md)