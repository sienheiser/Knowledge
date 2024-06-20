---
aliases: [basis of subspace]
---

Let $\mathcal{B}$ be a [[Basis for topology|basis]] for topology $\tau$ on $X$ and let $Y$ be a non-empty subset of $X$. Then collection 
$$
\mathcal{B}_Y = \{B\cap Y:B\in\mathcal B\}.
$$
Is a basis for subspace $(Y,\tau_Y)$.

*Proof:* Take $U_y\in\tau_Y$. There exists $U\in \tau$ such that $U_y = U\cap Y$. Since $\mathcal{B}$ is basis for $\tau$ we know 
$$
U = \bigcup_{i\in I}B_i
$$
where $I$ is an index set and $B_i\in\mathcal{B}$. Therefore 
$$
U_y = (\bigcup_{i\in I}B_i)\cap Y= (\bigcup_{i\in I}B_i\cap Y).
$$
We can see that $B_i\cap Y \in \mathcal{B}_Y$. Since $U_y$ is arbitrary $\mathcal{B}_Y$ is a basis for $\tau_Y$.