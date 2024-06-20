---
aliases: [open sets and neighbourhoods]
---

*Corollary:* Let $U$ be a subset of [[Axioms|topological space]] $(X,\tau)$. Then $U\in\tau$ if and only if for each $x\in U$ there exists [[Neighbourhood|neighbourhood]] $N$ of $x$ such that $N\subseteq U$.

*Proof:* Assume $U\in \tau$. For each $x\in U$, $U$ is a neighbourhood of $x$.
Assume that for each $x\in U$ a neighbourhood $N$ of $x$ such that $N\subseteq U$ exists. Then we label the neighbourhood for a $x$ as $N_x$. This means that exists open sets $V_x$ such that $x\in V_x\subseteq N_x\subseteq U$. Clearly, 
$$
U = \bigcup_{x\in U}V_x.
$$
Since $U$ is a union of open sets, then $U$ is an open set.

z