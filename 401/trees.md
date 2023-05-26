# Trees

### Binary Trees:

* A Binary Tree is a hierarchical data structure composed of nodes, where each node has at most two children: a left child and a right child. The topmost node is called the root node. Nodes in a Binary Tree can have zero, one, or two children.

* Think of a Binary Tree as a family tree, where each person represents a node. Each person can have at most two children (left and right), and the topmost person represents the root of the family tree.

### Binary Search Trees (BSTs):
* A Binary Search Tree is a type of Binary Tree with an additional property: the values in the left subtree of any node are less than the value of the node, and the values in the right subtree are greater than the value of the node. This property makes BSTs efficient for searching, inserting, and deleting elements.

* Imagine you have a collection of books arranged on a bookshelf. The books are organized in a way that for any given book, all the books to the left have lower values (e.g., lower ISBN numbers) and all the books to the right have higher values. This arrangement allows for quick searching and inserting of books based on their values.

### K-ary Trees:
* A K-ary Tree is a generalization of a Binary Tree, where each node can have up to K children. K is a positive integer. In a K-ary Tree, each node can have zero to K children, and the children are usually ordered.

* Imagine a company organization chart, where each employee is represented by a node. In a K-ary organization chart, each employee can have multiple subordinates (children). For example, in a 3-ary organization chart, each employee can have up to three direct subordinates, making it a tree structure where each node can have at most three children.

### Tree Cheat Sheet:

1. Tree: A hierarchical data structure composed of nodes.

   * Consists of a root node and zero or more child nodes.
   * Each child node can have its own child nodes, forming a recursive structure.
   * No cycles or loops are allowed in a tree.

2. Binary Tree:

   * Each node has at most two children: a left child and a right child.
   * Nodes can have zero, one, or two children.
   * Useful for representing hierarchical relationships.

3. Binary Search Tree (BST):

   * A Binary Tree with the following property:
     * For any node, the values in the left subtree are less than the node's value.
     * The values in the right subtree are greater than the node's value.
   * Enables efficient searching, insertion, and deletion operations.
   * In-order traversal of a BST visits nodes in ascending order.

4. K-ary Tree:

   * Each node can have up to K children.
   * K is a positive integer.
   * Generalization of Binary Trees.
   * Useful for representing hierarchical structures with multiple branches.

5. Common Tree Terminology:
     * Root: The topmost node in a tree.

     * Parent: The node directly above a given node.

     * Child: A node directly below another node.

     * Sibling: Nodes that share the same parent.

     * Leaf: A node with no children.
  
     * Height: The length of the longest path from the root to a leaf node.

     * Depth: The length of the path from a node to the root.

      * Subtree: A portion of a tree, consisting of a node and its descendants.