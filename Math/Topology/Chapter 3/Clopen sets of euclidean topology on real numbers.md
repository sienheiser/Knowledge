*Proposition:* Let $T$ be a clopen subset of $\mathbb{R}$. Then either $T=\mathbb{R}$ or $T=\emptyset$.

*Proof:* Suppose $T\neq\mathbb{R}$ or $T\neq\emptyset$. Then there exists an $x\in T$ and $z\in \mathbb{R}\backslash T$. WLOG, let $x<z$. Since $T$ is closed then we may construct closed set $S= T\cap [x,z]$. Clearly, $z$ is an upper bound of $S$ but does not belong to $S$ because $z\notin T$ by definiton. Let $p$ be the supremum of $S$. Then we know that $p\leq z$. By [[Supremum belongs to closed sets]] $p\in S$. Therefore $p<z$.

Since $T$ is an open set there exists real numbers $a,b$ such that $p\in (a,b)\subseteq T$. Now we may choose $t$ such that $p<t<\text{min}(b,z)$. Then $t\in T$. But $t\in[x,z]$ since $x<p<t<z$. Therefore $t\in S$. This is a contradiciton, because $p$ is the supremum of $S$. Therefore our supposition is false and $T=\mathbb{R}\lor T=\emptyset$.
