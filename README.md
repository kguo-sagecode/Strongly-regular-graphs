# SRGs
A repository of some strongly regular graphs, stored in g6 format. 

[Ted Spence's website](https://www.maths.gla.ac.uk/~es/srgraphs.php) has a large collection of strongly regular graphs on at most 64 vertices, with parameters which have been fully classified. This is a valuable resource for testing conjectures on strongly regular graphs. Towards the same end, I will collect strongly regular graph with parameters which have not been fully classified. 

For example, the parameter class (37,18,8,9) is not known to be fully classified. This class is not found on Ted Spence's website, but [Brendan McKay's website](https://users.cecs.anu.edu.au/~bdm/data/graphs.html) has 6760 graphs in this class.
For example, there are 4466 strongly regular graphs with parameters (63,32,16,16), coming from block graphs of block designs (the vertices are blocks and are adjacent if they intersect at a point). These block designs have parameters (v,b,r,k,lambda) = (28, 63, 9, 4, 1), which are Steiner design S(2, 4, 28) or partial geometries pg(3,8,4). The 4466 with non-trivial automorphism groups are given on [Vedran Krcadinac's website](https://web.math.pmf.unizg.hr/~krcko/results/steiner.html). See also:

Krčadinac, Vedran. (2002). Steiner 2-designs S(2,4,28) with nontrivial automorphisms. Glasnik Matematicki (glasnik@math.hr); Vol.37 No.2. 37. 

Here, we have compute the 4466 strongly regular graphs which are the block graphs of these 4466 Steiner designs and stored them as the graph6 string of the canonical labelling. Two graph are isomorphic if and only if the graph6 strings of the canonical labelling are equal. 

In "SRG63-32-16-16-S-2-4-28.txt", each line is a graph6 string (followed by "\n").

To read this using SageMath, do something like:

    sage: f = open("SRG63-32-16-16-S-2-4-28.txt","r")
    sage: g6s = f.readlines()
    sage: f.close()
    sage: gs = [Graph(g.strip("\n")) for g in g6s]

This will produce a list of the graph objects, called gs. 

## File names and contents

- SRG63-32-16-16-S-2-4-28.txt

4466 strongly regular graphs with parameters (63,32,16,16), coming from block graphs of block designs S(2, 4, 28). 

- SRG63-32-16-16-quasi.txt

These are the 3511 strongly regular graphs that are construct as the intersection-6 graphs (vx set = block, adjacent if intersect in 6 points) of the 89559 quasi-symmetric 2-designs with (v,b,r,k,lambda) = (28, 63, 27, 12, 11), where every pair of blocks intersects in either 4 or 6 points, which are given on [Vedran Krcadinac's quasi-symmetric designs website](https://web.math.pmf.unizg.hr/~krcko/results/quasisym.html).
