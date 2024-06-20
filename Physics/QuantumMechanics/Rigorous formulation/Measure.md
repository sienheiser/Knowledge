*Definiton:* A measure $\mu:\sigma\rightarrow \overline{\mathbb{R}^+}_0$ (where $\overline{\mathbb{R}} = \mathbb{R}\cup(-\infty,\infty)$) on a measurable space $(M,\sigma)$ is a map satisfying 
1. $\mu(\emptyset) = 0$
2. A sequence $A_1,A_2,...\in \sigma$ with $A_i\cap A_j = \emptyset\quad \forall i\neq j$ $$\mu(\bigcup_{n\geq 1}A_n) = \sum_{n\geq 1}\mu(A_n)  $$ 

Terminology: $(M,\sigma,\mu)$ is called a measure space.

### Properties of a measure

1. Monotony: $A_1\subseteq A_2\implies \mu(A_1)\leq\mu(A_2)$.
2. Sub additivity: $\{A_1,A_2,...\}\in\sigma\implies \mu(\bigcup_{n\geq 1}A_n)\leq\sum_{n\geq 1}\mu(A_n)$.
3. Continuity from below: Suppose $A_1\subseteq A_2 \subseteq...\implies \bigcup_n A_n = A$. Then $$\lim_{n\rightarrow \infty}\mu(A_n) = \mu(A)$$.
4. Continuity from above: Suppose $A_1\supseteq A_2\supseteq ...$  , $\bigcap_n A_n = A$ and $\mu(A_n)<\infty\quad \forall n\in\mathbb{N}$. Then $$\lim_{n\rightarrow \infty}\mu(A_n)= \mu(A)$$

Note for 4. we can prove that  $\bigcap_n A_n = A\in \sigma$ using deMorgon's rule.