---
aliases: [condition for subset to be dense]
---

*Proposition:* Let $A$ be a subset  of a [[Axioms|topological space]] $(X,\tau)$. Then $A$ is [[Math/Topology/Chapter 3/Dense|dense]] in $X$ if and only if every non-empty open subset of $X$ intersects $A$ non-trivially.

*Proof:* Assume that $A$ is dense in $X$. Suppose that there exists an open subset $U$ such that $A\cap U = \emptyset$. Then all elements of $U$ are not limit points of $A$. This means for any $x\in U$, $x\notin A'$ and $x\notin A$. Since $A\cup A' = X$ and $U\subseteq X$ this is a contradiciton because $X$ contains elements of $U$. Therefore such a set does not exist and all open subsets intersect with $A$ non-trivially.

Assume all open sets intersect with $A$ non-trivially. Then all the elements of $X\backslash A$ are [[Limit points|limit points]] of $A$. Because for any $x\in X\backslash A$ there exists an open set $U_x\ni x$. Since all open sets contains points of $A$, $x$ is a limit point of $A$. Now $A'$ is the set that contains all the limit points of $A$. Therefore $X\backslash A\subseteq A'$. Since $A\cup X\backslash A = X$ then $A\cup A' = X$. So $A$ is dense in $X$.