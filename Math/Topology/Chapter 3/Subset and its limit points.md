---
aliases: [subset and its limit points]
---
*Proposition:* Let $A$ be a subset of [[Axioms|topological space]] $(X,\tau)$ and $A'$ the set of all [[Limit points|limit points]] of $A$. Then $A\cup A'$ is a [[Open and Closed sets|closed set]].

*Proof:* We want to use proposition [[Closed set and limit points|closed set and limit points]]. Therefore we want to show that $X\backslash A\cup A'$ contains no limit points of $A\cup A'$.

Let $p\in X\backslash (A\cup A')$. As $p\notin A'$ there exists an open set $U$ such that $A\cap U=\emptyset$ or $\{p\}$. In this case $A\cap U = \emptyset$. We also claim that $A'\cap U=\emptyset$. Take any $x\in U$, then $A\cap U=\emptyset$ implies that $x\notin A'$. Therefore $A'\cap U=\emptyset$. Thus, $(A\cup A')\cap U = \emptyset$. Therefore $p$ is not a limit point $A$ and $A\cup A'$ is a closed set.

