---
aliases: [interval]
---

*Definition:* A subset $S$ of $\mathbb{R}$ is said to be an **interval** if it has the following property: if $x\in S$, $z\in S$, and $\exists y\in\mathbb{R}$ such that $x<y<z$, then $y\in S$.

*Remarks* 
1. Each singleton set $\{x\}$ is an interval
2. Every interval has one of the following forms: $\{a\},(a,b),[a,b],(a,b],[a,b),(-\infty, a),(-\infty, a],(a,\infty),[a,\infty),(-\infty,\infty)$.
3. Every interval is [[Homeomorphism|homeomorphic]] to $(0,1),[0,1],[0,1)$ or $\{0\}$.

### All intervals are connected
*Proposition:* A subspace $S$ of $\mathbb{R}$ is connected if and only if it is an interval. 

*proof:* Let $S$ be an interval. Suppose there exists proper non empty clopen subset $T$ of $S$. That is $T\neq S$ or $T\neq \emptyset$. Then $x\in T$ and $z\in S\backslash T$. WLOG let $x<z$. Now create another closed set $A=T\cap [x,z]$. This is a closed set.
	*proof:* Since $T$ is closed set of $S$. There exists closed set $U\subseteq\mathbb{R}$ such that $T=U\cap S$. Take any other closed subset, $V$, of $\mathbb{R}$. Then $V\cap S$ is a closed subset of subspace $S$. This means that $(V\cap S)\cap (U\cap S)$ is a closed subset of subspace $S$. But $(V\cap S)\cap (U\cap S) = S\cap(V\cap U)$ which is still a closed subset of subspace $S$. 

It is clear that $z$ is an upper bound of $A$. Let $p$ be the supremum of $A$. Then we know that $p\leq z$. By proposition [[Supremum belongs to closed sets]] $p\in A$. Therefore $p<z$.

Since $T$ is open and $p\in T$ there exists open interval $(a,b)$
$$
p\in (a,b)\subseteq T.
$$
We may choose number $t$ such that $p<t<\text{min}(z,b)$. Then $t\in T$, furthermore, $t\in[x,z]$ since $x < p< t<z$. Therefore, $t\in A$ which is a contradiction since $p$ was supposed to be the supremum. Hence $T$ cannot be a proper non empty clopen subset of $S$. 


Now assume that $S$ is connected. Suppose $x\in S,z\in S$ and $y\in\mathbb{R}$ such that $x < y< z$ but $y\notin S$.  Then set $(-\infty,y)\cap S= (-\infty,y]\cap S$ is open and closed.
	*proof:* Set $(-\infty,y)$ is open in $\mathbb{R}$. Therefore $(-\infty,y)\cap S$ is open in $S$. Set $(-\infty,y]$ is closed in $\mathbb{R}$. Therefore $(-\infty,y]\cap S$ is closed in $S$.

So $(-\infty,y)\cap S$ is a clopen subset of $S$. Now we show that it is a proper no empty subset of $S$. It is non empty since $x\in (-\infty,y)\cap S$, it  is a proper subset since $z\notin (-\infty,y)\cap S$. This is a contradiction since $S$ is a connected space. Therefore $S$ is an interval. 



