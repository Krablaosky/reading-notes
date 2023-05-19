# Linked List
Linked List Cheat Sheet:

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