# Forrest Gump Graph

## Week 1
- Draw the graph
- Compute the number of nodes,edges, average degree and the density. Comment.

## Week 2
While considering the largest component of your network. Depending on what you prefer/seems
more relevant in your graph,
- Compute Average distance and Diameter,
- Improve the function computing the inverse distance function.

Or

- Compute Average clustering and Transitivity number,
- Implement a function computing the transitivity using basic function of networkx

## Week 3
Depending on what seems more relevant in your graph, pick one of the following local notions

- Decay centrality

- Betweeness centrality

- Closeness centrality

- Clustering

- Any other notion that you invent

1) Provide a code computing the given notion using basic functions of networkx (you are not allowed to use directly the functions of networkx computing it).

2) Discuss why you picked this measure and who is the most central in your network based on your choice.

3) Provide the cumulative distribution for this centrality or the histogram and give a graphical representation of your graph (log-log, log or normal representation as you think it is more relevant).

## Week 5
1) Write a function to compute the PageRank of the nodes in a graph (you are not allowed to use built-in functions from NetworkX).

2) Run it on your graph using α = 0.15, save the total number of iterations, and check that your function returns the same results (in terms of the scores) as the built-in function from NetworkX.

3) Identify the node with the highest PageRank, compare it with the one you got from week 3, and give an interpretation to the possible difference.

4) Provide the cumulative distribution, compare it with the one you got from week 3, and comment the results. 

5) Optional: Re-run the PageRank using α = 0.5, save the total number of iterations, compare with the results (in terms of both the number of iterations and the cumulative distribution) obtained for α = 0.15, and comment.

Hint: treat weighted graphs as unweighted & links in undirected graphs as doubly directed (each undirected link becomes a directed link in both directions).
Additionally, make sure you run the PageRank algorithm on a connected graph.

## Week 6
0) Treat your graph as undirected and unweighted. Delete loops and work on the resulting largest
connected component.
1) Implement the following three techniques for community detection:
a) Bridge removal (pick the partition with the highest modularity), b) Modularity optimization, c) Label
propagation.
In this case, you are allowed to use built-in functions from NetworkX.
2) Compare the results of each technique in terms of: a) number of detected clusters, b) cluster sizedistribution, c) computational time, e) modularity, f) other aspects you consider relevant, if any. Resultsshould be presented in a table.
3) Give an interpretation to the differences and similarities between the three resulting partitions, anddiscuss which one you think is the best and why.
4) Provide a visualization for the partition you decided to be the best using Gephi.
5) Optional: for each pair of partitions compute the NMI between them and discuss.

## Week 7

0) Treat your graph as undirected and unweighted, and work on the resulting largest connected
component. Delete loops
1) Create a function computing CN and one of the topological indices between JI,PA,AA,RA.
Your function should return a pandaframe where each row is a missing link and each column is
an index. You are allowed to use built-in functions from NetworkX for computing individual
indices.
2) Create a third score by adding a column with the arithmetic mean between the two indices.
[NB: the arithmetic mean should be computed after rescaling each column between 0 and 1.]
3) For each of the 3 scores, identify as missing links the node pairs yielding the largest 5 values.
Briefly comment the results.
4) Optional: Invent a new index/score and compare the result