---
layout: archive
title: "Problems"
permalink: /problems/
author_profile: false
math: true
---
Here are some open problems I've spent some time thinking about. If you want to talk about any of these, please reach out!

## Total connectivity
For distinct vertices \\( u,v \\) in a graph \\( G \\) let \\( \kappa_G(u,v) \\) denote the largest number of internally disjoint \\( u \\)-\\( v \\) paths in $G$. The _total connectivity_ \\( T(G) \\) is defined as \\( \sum_{u,v \in V(G)} \kappa_)G(u,v) \\). The _average connectivity_ of \\( G \\)  is defined as \\( \frac{T(G)}{\binom{|V(G)|}{2}} \\).

We know that in any graph of average degree at least \\( 2d \\) has a subgraph of minimum degree at least \\( d \\). What is the analogous bound for average connectivity versus usual connectivity? In particular, for fixed \\( k>1 \\), how large can the average degree of a graph be without a \\( k \\)-connected subgraph. This question is trivial for \\( k=2 \\), but what about \\( k=3 \\)? Let \\( f(n) \\) denote the largest total connectivity of a graph on \\( n \\) vertices without a \\( 3 \\)-connected subgrapph. What is \\( f(n) \\)?

I think the answer is \\( f(n) = 2n^2-6n+7 \\) for \\( n \geq 5 \\). The hard part of this question is dealing with graphs that are subdivisions of \\( 3 \\)-connected graphs. 