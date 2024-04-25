# SRGs
A repository of some strongly regular graphs, stored in g6 format. 

[Ted Spence's website](https://www.maths.gla.ac.uk/~es/srgraphs.php) has a large collection of strongly regular graphs on at most 64 vertices, with parameters which have been fully classified. This is a valuable resource for testing conjectures on strongly regular graphs. Towards the same end, I will collect strongly regular graph with parameters which have not been fully classified. 

For example, there are 4466 strongly regular graphs with parameters (63,32,16,16), coming from block graphs of block designs (the vertices are blocks and are adjacent if they intersect at a point). These block designs have parameters (v,b,r,k,lambda) = (28, 63, 9, 4, 1), which are Steiner design S(2, 4, 28) or partial geometries pg(3,8,4). The 4466 with non-trivial automorphism groups are given on [Vedran Krcadinac's website](https://web.math.pmf.unizg.hr/~krcko/results/steiner.html). See also:

Krčadinac, Vedran. (2002). Steiner 2-designs S(2,4,28) with nontrivial automorphisms. Glasnik Matematicki (glasnik@math.hr); Vol.37 No.2. 37. 

Here, we have compute the 4466 strongly regular graphs which are the block graphs of these 4466 Steiner designs and stored them as the graph6 string of the canonical labelling. Two graph are isomorphic if and only if the graph6 strings of the canonical labelling are equal. 
