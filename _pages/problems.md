---
layout: archive
title: "Problems"
permalink: /problems/
author_profile: false
math: true
---
Here are some open problems I've spent some time thinking about. If you want to talk about any of these, please reach out!

## Connectivity vs average connectivity
For distinct vertices \\( u,v \\) in a graph \\( G \\) let \\( \kappa_G(u,v) \\) denote the largest number of internally disjoint \\( u \\)-\\( v \\) paths in $G$. The _total connectivity_ \\( T(G) \\) is defined as \\( \sum_{u,v \in V(G)} \kappa_G(u,v) \\). The _average connectivity_ of \\( G \\)  is defined as \\( \frac{T(G)}{\binom{|V(G)|}{2}} \\).

We know that in any graph of average degree at least \\( 2d \\) has a subgraph of minimum degree at least \\( d \\). What is the analogous bound for average connectivity versus usual connectivity? In particular, for fixed \\( k>1 \\), how large can the average degree of a graph be without a \\( k \\)-connected subgraph. This question is trivial for \\( k=2 \\), but what about \\( k=3 \\)? Let \\( f(n) \\) denote the largest total connectivity of a graph on \\( n \\) vertices without a \\( 3 \\)-connected subgraph. What is \\( f(n) \\)?

I think the answer is \\( f(n) = 2n^2-6n+7 \\) for \\( n \geq 5 \\). The hard part of this question is dealing with graphs that are subdivisions of \\( 3 \\)-connected graphs. 

## Ideally connected graphs
For distinct vertices \\( u,v \\) in a graph \\( G \\) let \\( \kappa_G(u,v) \\) denote the largest number of internally disjoint \\( u \\)-\\( v \\) paths in $G$. Note \( \kappa_G(u,v) \leq \min{ { \text{deg}_G(u), \text{deg}_G(v) }} \). If equality is attained for every pair of vertices in \( G \), then \( G \) is called ideally connected.

Given a graph class, what do the ideally connected graphs in the class look like? For instance, I showed that the ideally connected chordal graphs are precisely the threshold graphs, and the ideally connected cographs are the complements of trivially perfect graphs. What about other graph classes with nice decomposition properties, such as distance-hereditary circle graphs?

A related question is to determine graph operations that preserve ideal connectedness. Maybe it is possible to give a structural description of all ideally connected graphs in terms of known decomposition operations, such as gluing along a subgraph in a certain way, graph joins, subdivisions, etc.

## Graph partitioning with connectivity constraints
Thomassen conjectured that the vertices of any \( s + t + 1 \)-connected graph can be partitioned into two sets, the first inducing an \( s \)-connected graph and the second inducing a \( t \)-connected subgraph. Can we prove this for certain graph classes? One can show that the conjecture is equivalent to finding disjoint \( s \)- and \( t \)-connected subgraphs in the graph.

Maybe a good place to start is a graph class that ensures somewhat large cliques. For instance, if the graph class (such as chordal graphs) ensures a \( K_s \), then we're done. To make progress on this conjecture it will be necessary to find a way to guarantee a highly connected subgraph in a stronger way than using a density argument.