A *cut-set* in a graph is a set of edges whose removal breaks the graph into two or more connected components. Given a graph $G = (V, E)$ with $n$ vertices, the minimum cut – or *min-cut* – problem is to find a minimum cardinality cut-set in $G$. Min-Cuts also arise in clustering problems. In the context of machine communication, Min-Cut is the minimum amount of nodes that can fail before some pair of machines can't communicate. For example, if nodes represent Web pages (or any documents in a hypertext-based system) and two nodes have an edge between them if the corresponding nodes have a hyperlink between them, then small cuts divide the graph into clusters of documents with few links between clusters. Documents in different clusters are likely to be unrelated.

The algorithm has $n-2$ iterations. There is an edge contraction in each iteration. In the end, the graph consists of two vertices. The algorithm outputs the set of edges connecting the two remaining vertices.

It is easy to verify that any cut-set of a graph in an intermediate iteration of the
algorithm is also a cut-set of the original graph. On the other hand, not every cut-set of the original graph is a cut-set of a graph in an intermediate iteration, since some edges of the cut-set may have been contracted in previous iterations. As a result, the output of the algorithm is always a cut-set of the original graph, but not necessarily the minimum cardinality cut-set (see Figure 1.1).

![[Figure 1.1.png]]

## [[Theorem 1.8]] : 
*The algorithm outputs a min-cut set with probability at least $\frac{2}{n(n-1)}$.*