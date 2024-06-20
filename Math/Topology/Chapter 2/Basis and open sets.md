---
aliases: [basis and open sets]
---
*Proposition:* Let $\mathcal{B}$ be a basis for topology $\tau$ on a set $X$. Then a subset $U$ of $X$ is open if and only if for each $x\in U$ there exists a $B\in\mathcal{B}$ such that $x\in B\subseteq U$.

*Proof:* Let $\mathcal{B}$ be a basis for topology $\tau$ on a set $X$. Assume that $U$ is an open set. Then by definition of [[Basis for topology|basis]]
$$
U = \bigcup_{i\in I}B_i\quad\text{where }B_i\in\mathcal{B}
$$
where $I$ is an index set. Then for each $x\in U$ there exists some $B_j$ such that $x\in B_j\subseteq U$. 

Assume that for each $x\in U$ there exists a $B_x\in\mathcal{B}$ such that $x\in B_x\subseteq U$. Then we show that 
$$
U = \bigcup_{x\in U}B_x.
$$
Take any $y\in U$, then by assumption there exists $B_y$ such that $y\in B_y\subseteq U$. Therefore $y\in\bigcup_{X\in U}B_x$.

Take any $y\in\bigcup_{X\in U}B_x$. Then $y\in B_j$ for some $j$. Since $B_j\subseteq U$ then $y\in U$.