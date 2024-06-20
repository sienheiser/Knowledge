---
aliases: [basis for a given topology]
---

*Proposition:* Let $(X,\tau)$ be a topological space. A family $\mathcal{B}$ of open subsets of $X$ is a basis for $\tau$ if and only if for any point $x$ belonging to any open set $U$, there is a $B\in\mathcal{B}$ such that $x\in B\subseteq U$.

*Proof:* Let $\mathcal{B}$ be a collections of open subsets of $X$. Assume that $\mathcal{B}$ is a basis for $\tau$. Then any $U\in \tau$ can be written as 
$$
U = \bigcup_{i\in I}B_i\quad\text{where }B_i\in\mathcal{B}
$$
and $I$ is an index set. Now take any $x\in U$, then $x\in B_j$ for some $j\in I$.  Therefore we have found a $B_j\in\mathcal{B}$ such that $x\in B_j\subseteq \mathcal{B}$.

Now assume that for any point $x$ belonging to any open set $U$, there is a $B\in\mathcal{B}$ such that $x\in B\subseteq U$. Take an open set $V$. We know for each $x\in V$ there exists a $B_x\in\mathcal{B}$ such that $x\in B_x\subseteq V$. If we show that 
$$
V = \bigcup_{x\in V}B_x
$$
then we have shown that $\mathcal{B}$ is a basis for $\tau$ since $V$ is a union of memebers of $\mathcal{B}$.  

Take any $y\in V$ then there exists $B_y$ such that $y\in B_y\subseteq V$. Therefore, $y\in\bigcup_{x\in V}B_x$. 
Take any $y\in\bigcup_{x\in V}B_x$, then there exists $B_y$ such that $y\in B_y\subseteq V$. 

