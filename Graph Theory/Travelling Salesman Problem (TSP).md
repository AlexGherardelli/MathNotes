---
subject: computer science
tags:
  - computer-science
  - math
parent: [[Math & Tehroetical Computer Science MOC]]
related_pages:
 - [[Illustration MOC]]
 - [[Topics to research]]
---

Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city exactly once and returns to the origin city?

![Pasted image 20241004162932.png](assets/Pasted%20image%2020241004162932.png)

Also more formally: given a complete [[Graph theory |graph]] with weighted edges (as an [[Graph theory |adjacency matrix]]) what is the [[Hamiltonian cycle]] of minimum cost?

The optimal solution to the TSP problem is **very hard**,as the problem is known to be [[P vs NP| NP-Complete]]. There are however approximations that will make algorithms work very fast 

## Brute force solution
Listing all possible permutations of node orderings. Very bad outcome which takes $O(n!)$ time

## Dynamic programming
Improves the runtime to $O(n^2 2^n)$
This makes it possible to compute a solution for ~23 nodes on a home computer.
