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

# Connectivity and Path

Can we get from one point to another?
Is there a relationship link between two people?
What connected groups does a person belong to?
Which one scientific paper influenced by another?

## Paths
從v0開始，連接到vn的路線。
A path from vertex v0 to vn is a sequence of edges that connect successive vertices in a sequence v0, v1, v2... vn. The path length is n.


![path](./path.png)

1. (a, b), (b, c), (c, e)
2. (a, b), (b, c), (c, e), (e, b), (b, c), (c, e)


A path is "simple" if it does not have repeated deges. 

### Circuit

A "circuit" is a path that starts and ends with the same vertex.


- Simple Circuit: (b,c), (c,e), (e,b)
- Non-Simple Circuit: (b,c) (c,e) (e,b) (b,c) (c,e) (e,b)

## Simple Path Lemma
Lemma: If there is a path between vertices u and v in a graph, then there is a simple path between u and v.

P: There is a path between u and v
Q: There is a simple path between u and v

Need to prove P -> Q

Assume that P is true.

#### Case1: Path is simple. Then Q is True.
#### Case: Path is not simple.
We get a repeated path from u to v.
- (u,a) (a,v) (v,b) (b,a) (a,v)
- We repeated (a,v) twice. There is a "circuit".(Start at A and end up A)
- We can cut the circut out of the path and still get the path we want.

***

# Connectedness 
無向圖中，每兩點間都有一個Path連接，就是Connected.
An undirected graph is called connected if there is a path "between every pair of distinct vertices" in the graph.
有向圖中，strongly connected必須讓每個點都能有a到b與b到a的路徑。

## Connectedness Theorem
Undirected graph G is connected if and only if there is a simple path between each pair of vertices in G.

P = G is connected
Q = Simple path between each pair of distinct vertices in G

#### P -> Q
Assume P is true. Thus, there is a path between each pair of vertices.
Thus, by simple path Lemma, each pair has a simple path.
Q is true.


#### Q -> P

Assume that Q is true. Then there is a simple path between each pair of vertices. So, P is true by definitions of Connectedness.

***

## Directed Graph
A directed path in a directed graph G from vertex v0 to vn is sequence of edges that connect successive vertices(order matters) in a sequence v0, v1, v2...vn.

![DirectedPath](./directedPath.png)

- Directed paths from a to e: (a,b) (b,e)
- No directed path from a to c
- No directed path form e to any vertex.


## Strongly Connected Directed Graph
A directed graph is strongly conected if for each pair of vertices there is a directed path from u to v and from v to u.

- Indicators of communities in social networks.

***

## Path, Trails, Circuits and Conectivity

| Name | Repeated Edge | Repeated Vertex | Starts and Ends at same point | Must contain at least one edge|
|------|---------------|-----------------|-------|-----|
| Walk | Allowed       | Allowed         | Allowed| No|
| Trail| No       | Allowed         | Allowed| No|
| Path | No       | No         | No |  No|

***

[Walks, Trails, Paths, Circuits](http://mathonline.wikidot.com/walks-trails-paths-cycles-and-circuits)

## Walks

Definition: For a graph G=(V(G),E(G)), a Walk is defined as a sequence of alternating vertices and edges such as v0,e1,v1,e2,...,ek,vk where each edge ei={vi−1,vi}. The Length of this walk is k.

Note that walks can have repeated edges.

## Open / Closed Walks

Definition: A walk is considered to be Closed if the "starting vertex is the same as the ending vertex", that is v0=vk. A walk is considered Open otherwise.

## Trails
A Trail is defined as a walk with no repeated edges.

## Paths
Definition: A Path is defined as an open trail with no repeated vertices.

Notice that all paths must therefore be open walks, as a path "cannot both start and terminate at the same vertex."

## Circuit
Definition: A Circuit is a "closed trail". That is, a circuit has no repeated edges but may have repeated vertices.

***
## Euler Circuirs

Let G be a graph. An Euler Circuit for G is a circuit that contins every vertex and every edge of G. That is, an Euler circuit for G is a sequence of adjacent vertices and edfes in G that has at least one edge, starts and ends at the same vertex, "uses every vertex of G at least once, and uses every edge of G exactly once".

***
## Required Reading
pp.  625-638 (Discrete Mathematics with Applications, Susanna S.Epp)
pp.  642-653 (Discrete Mathematics with Applications, Susanna S.Epp)
