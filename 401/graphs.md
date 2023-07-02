# Graphs

Think of a graph as a social network, where people are represented by vertices (nodes) and their relationships are represented by edges. Each person (vertex) in the network can be connected to one or more other people (adjacent vertices) through friendships (edges).

#### Terminology

- **Vertex**: A person in the social network.
- **Edge**: A friendship/connection between two people.
- **Neighbor**: Friends/connections of a person.
- **Degree**: The number of friends/connections a person has.

**Undirected Graph**:
An undirected graph is like a group of friends hanging out together. Everyone is connected to everyone else, and the friendships are bi-directional. If person A is friends with person B, then person B is also friends with person A.

**Directed Graph**:
A directed graph is like a network of followers on social media. People can follow others, but it doesn't mean that the other person follows them back. The connections have a specific direction.

**Complete Graph**:
A complete graph is like a group of friends where everyone is friends with everyone else. It's a tightly knit group where every person is connected to every other person.

**Connected Graph**:
A connected graph is like a group of friends where everyone is somehow connected to each other. Even if they are not direct friends, there is a path of friendships between any two people in the group.

**Disconnected Graph**:
A disconnected graph is like several separate groups of friends that have no connections between them. Each group has its own set of friendships, but there are no connections between the groups.

**Acyclic Graph**:
An acyclic graph is like a family tree. It represents a hierarchy where each person has a parent, and there are no loops or cycles in the relationships.

**Cyclic Graph**:
A cyclic graph is like a group of friends who form loops in their friendships. There are paths that can be followed that eventually lead back to the starting point.

**Weighted Graph**:
A weighted graph is like a network where friendships have different strengths or values assigned to them. The weights represent the level of closeness or importance of the connections.

**Traversal**:
Traversing a graph is like exploring social connections. Breadth-first traversal is like meeting people level by level, starting with your immediate friends and gradually expanding to friends of friends. Depth-first traversal is like diving deep into a specific person's connections and exploring their network before moving on to others.

**Graphs in Real Life**:
Graphs have many real-world applications. Just as social networks connect people, graphs can represent connections in GPS and mapping, driving directions, airline traffic, recommendations in online platforms like Netflix, and more.

## Cheat Sheet

**Graphs**
- Collection of vertices connected by edges.
- Vertices: Nodes in the graph.
- Edges: Connections between nodes.
- Directed vs Undirected.
- Complete vs Connected vs Disconnected.
- Acyclic vs Cyclic.

**Graph Representation**
-

 Adjacency Matrix: 2D array indicating edge connections.
- Adjacency List: Linked lists or arrays representing connected vertices.

**Weighted Graphs**
- Assign weights to edges representing cost or distance.

**Traversals**
- Breadth First Traversal: Visit vertices level by level.
- Depth First Traversal: Explore vertices deeply before backtracking.

**Real-World Uses of Graphs**
- GPS and Mapping.
- Driving Directions.
- Social Networks.
- Airline Traffic.
- Netflix Recommendations.

