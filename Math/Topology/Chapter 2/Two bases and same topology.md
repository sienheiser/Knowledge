*Proposition:* Let $\mathcal{B}_1$ and $\mathcal{B}_2$ be bases for topologies $\tau_1$ and $\tau_2$ respectively, on a non empty set $X$. Then $\tau_1$ = $\tau_2$  if and only if 
(i) for each $B\in\mathcal{B}_1$ and each $x\in B$, there exists $B'\in\mathcal{B}_2$ such that $x\in B'\subseteq B$ and,
(ii) for each $B\in\mathcal{B}_2$ and each $x\in B$, there exists $B'\in\mathcal{B}_1$ such that $x\in B'\subseteq B$.


*Proof:* Suppose that $\tau_1=\tau_2$. Since $\mathcal{B}_1$ is a basis for $\tau_1$ we know that each member of $\mathcal{B}_1$ is an open set in $\tau_1$. Take any $B\in\mathcal{B}_1$ then by propsition [[Basis for topology|basis for topology]] there exists $B'\in\mathcal{B}_2$ such that $x\in B'\subseteq B$. The same is true for the other way around. Therefore (i) and (ii) are true.

Suppose that (i) and (ii) are true. Then by proposition [[Basis and open sets|basis and open sets]] we know that (i) implies that memebers of $\mathcal{B}_1$ are open sets of $\tau_2$ i.e. $\mathcal{B_1}\subseteq\tau_2$. This means that $\tau_1\subseteq\tau_2$. Similarly, (ii) implies that $\tau_2\subseteq\tau_1$. Therefore $\tau_1=\tau_2$.

