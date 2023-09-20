## Graphs 

A Graph is a non-linear data structure consisting of vertices and edges. The vertices are sometimes also referred to as nodes and the edges are lines or arcs that connect any two nodes in the graph. More formally a Graph is composed of a set of vertices( V ) and a set of edges( E ). The graph is denoted by G(E, V).


### Analogy 

**Example: Family Tree as a Simple Graph**

Imagine you have a family tree like this:

- Node A represents Grandma.
- Node B represents Mom.
- Node C represents Dad.
- Node D represents You.
- Edges connect Grandma (A) to Mom (B) and Dad (C), indicating that Grandma is their parent.

Here's how it relates to a simple JavaScript graph:

- **Nodes**: A, B, C, and D are like different people or entities in your family.

- **Edges**: The connections between A and B, and A and C, are like the relationships or connections in your family tree.

- **Traversal**: You can traverse the graph to find out who your grandparents are. Starting from node D (you), you follow the edge to node B (Mom), and then the edge to node A (Grandma). So, you discover that A is your Grandma.


