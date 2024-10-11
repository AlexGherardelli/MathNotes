Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city exactly once and returns to the origin city?

![Pasted image 20241004162932.png](Pasted image 20241004162932.png.md)

Also more formally: given a complete [graph](Graph theory.md) with weighted edges (as an [adjacency matrix](Graph theory.md)) what is the [Hamiltonian cycle](Hamiltonian cycle.md) of minimum cost?

The optimal solution to the TSP problem is **very hard**,as the problem is known to be [ NP-Complete](P vs NP.md). There are however approximations that will make algorithms work very fast 

## Brute force solution
Listing all possible permutations of node orderings. Very bad outcome which takes $O(n!)$ time

## Dynamic programming
Improves the runtime to $O(n^2 2^n)$
This makes it possible to compute a solution for ~23 nodes on a home computer.
