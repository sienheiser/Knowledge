---
aliases: [limit point, limit points]
---

*Definition:* Let $A$ be a subset of [[Axioms|topological space]] $(X,\tau)$. A point $x\in X$ is said to be a limit point of $A$ if every open set, $U$, containing $x$ contains a point $A$ different from $x$.

e.g. Let $X=\{a,b,c,d,e\}$, $\tau = \{X,\emptyset,\{a\},\{c,d\},\{a,c,d\},\{b,c,d,e\}\}$ and $A = \{a,b,c\}$. 
We will cycle through all the points of $X$ and see which points are limit points of $A$.

1. $a\in X$, We see that $\{a\}\in\tau$ which is an open set containing $a$ but not a point of $A$ different $a$. Therefore $a$ is not a limit point of $A$.
2. $b\in X$, we see that the only open set containing $b$ is $\{b,c,d,e\}$ that also contains $c$ which is a point of $A$ different from $b$. Therefore $b$ is a limit point of $A$.
3. $c\in X$, we see that $\{c,d\}\in\tau$ is an open set containing $c$ but not a point of $A$ different from $c$. Therefore $c$ is not a limit point of $A$.
4. $d\in X$, we see that $\{c,d\},\{a,c,d\},\{b,c,d,e\}\in\tau$, all these sets containing $d$ contain a point of $A$ different from $d$. Therefore $d$ is a limit point of $A$.
5. $e\in X$, we see that $\{b,c,d,e\}\in\tau$ is the only open set containing $e$. It also contains a point of $A$ different from $e$. Therefore $e$ is a limit point of $A$.

