# Stacks and Queues

## [What are Stacks and Queues?](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)

### Here is the critical information you would need to understand what Stacks and Queues are.

Stacks:

  1. LIFO Principle: Stacks follow the Last-In-First-Out (LIFO) principle, meaning the last element added to the stack will be the first one to be removed.
  2. Push and Pop Operations: Elements are added to the top of the stack using the "push" operation and removed from the top using the "pop" operation.
  3. Main Operations: The main operations in a stack are "push" (add an element to the top) and "pop" (remove the top element).
  4. Stack Overflow and Underflow: Stack overflow occurs when trying to push an element onto a full stack, and stack underflow occurs when trying to pop from an empty stack.
  5. Applications: Stacks are useful in various scenarios, such as function calls and recursion, undo/redo operations, and expression evaluation.

Queues:

  1. FIFO Principle: Queues follow the First-In-First-Out (FIFO) principle, meaning the first element added to the queue will be the first one to be removed.
  2. Enqueue and Dequeue Operations: Elements are added to the rear of the queue using the "enqueue" operation and removed from the front using the "dequeue" operation.
  3. Main Operations: The main operations in a queue are "enqueue" (add an element to the rear) and "dequeue" (remove the front element).
  4. Queue Overflow and Underflow: Queue overflow occurs when trying to enqueue an element into a full queue, and queue underflow occurs when trying to dequeue from an empty queue.
  5. Applications: Queues are commonly used in scenarios like handling requests in web servers, breadth-first search algorithms, and task scheduling.


### Example Walkthroughs:

Stack Example Walkthrough:

  Think about a stack of books. You start by placing book A on top, then book B, and finally book C. Now, if you want to remove a book, you can only remove the one on top first (LIFO principle). So, when you pop a book from the stack, you'll get book C. The next pop will give you book B, and finally, the last pop will give you book A.

Queue Example Walkthrough:
  
  Imagine a queue of people waiting in line for a movie theater. The first person to arrive is at the front of the queue, and the last person to arrive is at the rear. When the theater opens, the person at the front of the queue enters first (FIFO principle). If you want to remove a person from the queue, you will always remove the one at the front. So, the first dequeue operation will give you the person at the front, the second dequeue will give you the next person, and so on.






