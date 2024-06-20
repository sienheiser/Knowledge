---
aliases: [proposition for euclidean topology on real numbers]
---

*Proposition:* Let $(\mathbb{R},\tau)$ be a [[Axioms|topological space]] with [[The Euclidean Topology on Real numbers|euclidean topology on real numbers]]. A subset $S$ is an [[Open and Closed sets|open set]] if and only if it is a union of open intervals.

*proof:* We have to assume that $S$ is an open set then show that it is a union of open intervals. Afterthat we have to assume that $S$ is a union of open intervals and show that it is an open set. 

We start by assuming that $S$ is a union of open intervals. From [[Open Sets and Closed Sets in The Euclidean Topology|open sets and closed sets of euclidean topology]] remark 1. We know that all open intervals on $\mathbb{R}$ are open sets. This means that $S$ is a union of [[Open and Closed sets|open sets]]. By the [[Axioms|axioms]] and [[Proposition for open and closed sets]] since  $(\mathbb{R},\tau)$ is a topological space we know that a union of open sets is still an open set. Therefore $S$ is an open set.

We assume that $S$ is an open set. Since $S$ is an open set we know it satifies that definion of [[The Euclidean Topology on Real numbers|euclidean topology on real numbers]]. This means for every $x\in S$ there exists an open interval $I_x$ such that $x\in I_x\subseteq S$. Suppose we define the set $\bigcup_{x\in S}I_x$ then we want to show that $S=\bigcup_{x\in S}I_x$. Start by taking $x\in S$ then we know that $x\in I_x$. This means that $x\in\bigcup_{x\in S}I_x\implies \bigcup_{x\in S}I_x\subseteq S$. 

Now take a $y\in\bigcup_{x\in S}I_x$. Then we know that $y\in I_t$ for some $t\in S$. Since $I_x\subseteq S$ for all $x\in S$ then $I_t\subseteq S$. This implies that $y\in S$ Therefore we have shown that $S\subseteq\bigcup_{x\in S}I_x$.

Since we have shown $S \subseteq \bigcup_{x\in S}I_x$ and $\bigcup_{x\in S}I_x\subseteq S$, this means $S = \bigcup_{x\in S}I_x$.