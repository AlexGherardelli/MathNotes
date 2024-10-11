# Main ideas
- 

# Summary
**Graphs**: It is a network that helps define and and visualize relationships (edges) between various components (nodes/vertex)

**Graph theory** is the study of these graphs and their properties. Graphs shows all the time like mapping, social networks

## Definitions

>  A graph $G = (V, E)$ is a a set of vertices $V$ and edges $E$ where each edge $(u, v)$ is a connection between vertices $u, v \in V$ 

*Example*: $V = \{1, 2, 4, 5 \}$ and $E = \{ (0, 1), (0, 2), (0, 3)\}$
#### **Neighbours**
Verteces $u$ and $v$ are neighbors f an edge $(u, v)$ connects them 
#### **Degrees**
Degree is equivalent of the number of neighbors of a node. 
#### **Path**
Sequences of verteces connected by edge. Path lenght = number of edges in a path
#### **Cycle**
Path that starts and end at the same vertex
#### **Connectivity**
Two verteces are connected if a path exists between them. A graph is called connected if when all verteces are connected.

*Connected component* a subset of vertices $V_i \subseteq V$ that is connected
#### **Undirected graph**
$(u, v) \implies (v, u)$
#### **Directed graph**
Edges are unidirectional
	- Directed cyclic graph
	- Directed acyclic graph

Edges are not considered equal and they have weights!
## Trees
Trees are subset of graphs with three specific properties:
1. Connected and acyclic
2. Removing an edge would disconnect the graph
3. Adding an edge would create a cycle
## Graph Representations
- **Adjency matrix**


![[complete-matrix.png]]

**Edge set**
![[A-graph-G-is-described-by-a-vertex-set-VG-and-an-edge-set-EG-A-A-simple.jpg]]

**Adjency list**
Very common, memory-efficient way of represent graphs, especially *sparse graphs* i.e. graphs with many nodes and not that many edges

![[adjacency_list.png]]

