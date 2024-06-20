---
aliases: [closed sets and neighbourhoods]
---

*Corollary:* Let $A$ be a subset of a [[Axioms|topological space]] $(X,\tau)$. Then $A$ is a [[Open and Closed sets|closed set]] if and only if for each $x\in X\backslash A$ there is a [[Neighbourhood|neighbourhood]] $N$ of $x$ such that $N\subseteq X\backslash A$.

*Proof:* Assume that $A$ is a closed set. Then by [[Closed set and limit points|closed set and limit points]] $A$ contains all its limit points. Set $X\backslash A$ does not have any limit points of $A$. This means for each $x\in X\backslash A$, there exists open sets $U$ that contain $x$ and no points of $A$. Such an open set is also a neighbourhood of $x$. Therefore we have found neighbourhood $U\subseteq X\backslash A$.

Assume that for each $x\in X\backslash A$ there is a neighbourhood $N$ of $x$ such that $N\subseteq X\backslash A$. This means for each $x$ there is a neighbourhood $N_x$. Furthermore, there exists open sets $U_x$ such that $x\in U_x \subseteq N_x\subseteq X\backslash A$. We show that

$$
X\backslash A = \bigcup_{x\in X\backslash A}U_x.
$$
Take any $y\in X\backslash A$. Then we know there exists open set $U_y\ni y$. Therefore, $y\in\bigcup_{x\in X\backslash A} U_x$ impying $X\backslash A \subseteq \bigcup_{x\in X\backslash A}U_x$.  

Take any $y\in\bigcup_{x\in X\backslash A}U_x$. Then for some $j$, $y\in U_j$. Since $U_j\subseteq X\backslash A$, $y\in X\backslash A$ which implies that $\bigcup_{x\in X\backslash A}U_x\subseteq X\backslash A$.

Since $X\backslash A$ is a union of open sets, $X\backslash A$ is an open set. Therefore $A$ is a closed set.