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
