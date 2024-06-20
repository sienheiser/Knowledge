---
aliases: [euclidean topology on real numbers]
---

*Definiton:* A subset $S$ of $\mathbb{R}$ is said to be an [[Open and Closed sets|open set]]  in the **euclidiean topology on $\mathbb{R}$** if it has the following property:
$$
(*)\ \ \ \ \text{For each}\ x \in S, \text{there exists}\ a,b,\in\mathbb{R},\ \text{with}\ a<b,\ \text{such that}\ x\in(a,b)\subseteq S.
$$
We have to show that the defined topology on $\mathbb{R}$ satisfies the [[Axioms|axioms]].

*Proof:* We show that $\mathbb{R}\in \tau$. Take $x\in \mathbb{R}$ then set $a=x-1$ and $b=x+1$. Clearly, $x\in(a,b)\subseteq\mathbb{R}$; that is $\mathbb{R}$ has propert $(*)$. Next we show that $\emptyset\in\tau$. There is nothing in $\emptyset$ therefore we do not need to take any $x\in\emptyset$ and find $a,b\in\mathbb{R}$. It is satisfied automatically???

Now we need to show that the union between open sets is an open set. let $x\in$ $\bigcup_{i\in I}S_i$ where $S_i$ are open sets. Then $x\in S_k$ for some $k\in I$. Since $S_k$ is an open set it satisfies property $(*)$ i.e. there exists $a,b\in\mathbb{R}$ such that $x\in(a,b)\subseteq S_k$. Then $x\in(a,b)\subseteq\bigcup_{i\in I}S_i$.  Therefore the second axiom is satisfied. 

Finally we need to show that the intersection between any two open sets is an open set. Take any two open sets $S_i,S_j$. Their intersection is $S_i\cap S_j$. Let $x\in S_i\cap S_j$. Then $x\in S_i$ and $x\in S_j$. Therefore there must exists $a,b,c,d\in\mathbb{R}$ such that $x\in(a,b)\subseteq S_i$ and $x\in(c,d)\subseteq S_j$. Let $e=\text{max}\{a,c\}$ and $f=\text{min}\{b,d\}$. Then $e<x<f$ and $(e,f)\subseteq S_i\cap S_j$. Therefore $x\in(e,f)\subseteq S_i\cap S_j$. Hence $S_i\cap S_j$ has property $(*)$ and so is in $\tau$. Therefore the definiton for the euclidean topology is a topology.