# Graph
A graph is a collection of vertices (Nodes) connected by edges (arcs)
A common abstract data type in CS.

## Simple Graph
A simple graph with no 'self loops' and at most one edge between an two vertices.

Formally a graph G is a specified by a pair(V, E) where V is a finite set of vertices and E is a set of edges. Each edge species a pair of vertices that it connects.

V = {a, b, c, d, e}
E = {(a,b), (b,c), (c,e), (e,b)} -> Oreder is not matter 

## Directed Graphs
有向圖
A directed graphs (V, E) specifies a set of vertices V and directed edges E. A directed edge is an oredered pair of vertices (a, b) denoteing an edge "going from" vertex a to vertex b

V = {a, b, c, d, e}
E = {(a,b), (b,c), (c,e), (e,b)} -> Oreder matters (a,b) != (b,a)


## Vertex Degree
有多少個edges連向特定的點
The degree of a vertax v(denoted deg(v)) in an undirected graph is the number of edges adjacent to v.

 ```
    b
  / |  \
a   |    c
    e   d

 ```

 deg(a) = 1
 deg(b) = 3
 deg(e) = 1
 deg(c) = 1
 deg(d) = 0

 ### Handshaking Property
 在無向圖中，有幾個edge就有 2 * edge 個 degree 總和。

 If an undirected graph(V, E) has e edges, then
 2 * e = sum of whole deg(v)

there are 3 edges in above graph, so the sum of the degree is 6 = 1 + 3 + 1 + 1 + 0

### Proof by Handshaking Property
Any undirected graph must have an even number of vertices with odd degree. (Zero is considered as even)

(By contradiction) Assume for the sake of contradiction that graph  G has an odd number of vertices with odd degree.

sum of the deg(v) = deg(odd) + deg(even) = odd value + even value = odd value 

By Handshaking Property, the sum of the degree should be even not odd value

***
## Bipartite Graph
兩個Set之內的Node間，沒有互相連接
a Graph that can be divided to two sets of vertices V1 and V2 such that there are no edges between nodes in V1 or between nodes in V2.

```
V1     V2
O -----O
  \
   \ 
    \ 
     \
O ---- O
O ---- O
```
### Example
Vertices in V1 are a set of jobs
Vertices in V2 are a set of workers
edges represent assignments of workers to jobs

### How can we tell if a graph is bipartite?
A two coloring of a graph is an assignment of one of Two colors to each vertex.

A graph is bipartite if and only if it has a two coloring such that no two vertices connected by an edge have the same color.

### Proof (Two colloring)
P = 'graph G is bipartite'
Q = 'G has 2 - coloring without edges between same color nodes'

Need to prove both 1) P -> Q 2) Q -> P

1) P -> Q

Assume P is true. We know the graph could be divided into two set.
Color vectices in V1 red color and in V2 black.
And its clear that Q is true, all the same color in the same set.

2) Q -> P

Assume Q is true. There is a two coloring graph.
Let V1 contain red vertices and V2 contian black vertices.

We see that P is true

***

## Required Reading
pp.  625-638 ( Discrete Mathematics with Applications, Susanna S.Epp)
***