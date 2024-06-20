---
aliases: [closed set and limit points]
---

*Proposition:* Let $A$ be a subset of [[Axioms|topological space]] $(X,\tau)$. $A$ is a [[Open and Closed sets|closed set]] if and only if $A$ contains all its [[Limit points|limit points]].

*Proof:*  Assume that $A$ is a closed set. Then by definiton [[Open and Closed sets|closed sets]] $X\backslash A$ is an open set. Suppose that $X\backslash A$ contains a limit point, $p$, of  $A$. Then for $p$ to be a limit point of $A$, $X\backslash A$ needs to have a point of $A$ different from $p$. But this is a contradiction as $X\backslash A$ does not have any points of $A$. Therefore $X\backslash A$ does not have any limit points of $A$ and as a consequence $A$ contains all its limit points.

Assume that $A$ contains all its limit points. Let us look at $X\backslash A$. We know it does not contains any limit points $A$, by assumption. This means for each $x\in X\backslash A$, there is an open $U_x$ that contains $x$ but no points $A$ different from $x$. We guess that 
$$
X\backslash A=\bigcup_{x\in X\backslash A} U_x
$$
$\quad\quad$*Proof*: Take any $y\in X\backslash A$. Then we know there is an open set $U_y\ni y$. Therefore $\quad\quad\quad\quad\quad y\in\bigcup_{x\in X\backslash A}U_x$.
$\quad\quad\quad\quad$ Take any $y\in\bigcup_{x\in X\backslash A}U_x$, then for some $j$ $U_j\ni y$, but $y\in U_j\subseteq X\backslash A$.
We have shown that $X\backslash A$ is a union of open sets. By the [[Axioms]] $X\backslash A$ is also an [[Open and Closed sets|open set]].

