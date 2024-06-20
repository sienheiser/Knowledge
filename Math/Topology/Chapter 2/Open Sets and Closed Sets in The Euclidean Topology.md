---
aliases: [open sets and closed sets of euclidean topology]
---
1. Let $r,s\in\mathbb{R}$ with $r<s$. In the [[The Euclidean Topology on Real numbers|euclidean topology]] $\tau$ on $\mathbb{R}$, the open interval $(r,s)$ belongs to $\tau$ and so is an [[Open and Closed sets|open set]].

*proof:* We need to show that $(r,s)$ has property $(*)$ from the definiton of [[The Euclidean Topology on Real numbers|euclidean topology]]. Let $x\in(r,s)$, set $a=r$ and $b=s$. Then $x\in(a,b)\subseteq(r,s)$. Therefore $(r,s)$ is an open set.

2. The open intervals $(-\infty,r)$ and $(r,\infty)$ are open sets for every real number $r$.

*proof:* We start by showing that $(r,\infty)$ is an open set for the euclidean topology on real numbers. Let $x\in(r,\infty)$. Then choose $a=r$ and $b=x+1$. Clearly, $x\in(a,b)\subseteq(r,\infty)$. Therefore $(r,\infty)$ is an open set. The same method can be used to prove that $(-\infty,r)$ is an open set.

3. While every open interval in $\mathbb{R}$ is an [[Open and Closed sets|open set]], not every open set in the [[The Euclidean Topology on Real numbers|euclidean topology]] is an open interval in $\mathbb{R}$.

*Example:* $(1,3)\cup(5,6)$ is an open set in $\mathbb{R}$, but not an open interval.

4. For $c,d\in\mathbb{R}$ with $c<d$, the closed interval $[c,d]$ is not an open set in $\mathbb{R}$.

*proof:* We do a proof by contradiction. We know $c\in[c,d]$. Assume there exists $a$ and $b$ such that $c\in(a,b)\subseteq[c,d]$. Now  $c\in(a,b)\implies a<c<b\implies a<\frac{a+c}{2}<c<b$. Therefore $\frac{a+c}{2}\in(a,b)$ but $\frac{a+c}{2}\notin [c,d]$. Hence $(a,d)\nsubseteq[c,d]$ which is a contradiciton. Therefore, such $a,b$ does not exist and $[c,d]$ does not have property $(*)$ from the [[The Euclidean Topology on Real numbers|euclidean topology]].

5. For each $a,b\in\mathbb{R}$ with $a<b$, the closed interval $[a,b]$ is a [[Open and Closed sets|closed set]].

*proof:* Clearly $\mathbb{R}\backslash[a,b]=(-\infty,a)\cup(b,\infty)\in\tau$ where $\tau$ is the [[The Euclidean Topology on Real numbers|euclidean topology]] on the real numbers.

6. Each singleton set is closed in $\mathbb{R}$

*proof:* Same resoning as in (5).

7. The set of all integers $\mathbb{Z}$ is a closed subset of $\mathbb{R}$

*proof:* $\mathbb{R}\backslash\mathbb{Z}=\bigcup_{i=-\infty}^{\infty}(n,n+1)$ is an open set.

8. The set $\mathbb{Q}$ is not an open or a closed subset of $\mathbb{R}$.


*proof:* We show that $\mathbb{Q}$ is not open. Let $x\in\mathbb{Q}$. Then we need to show that there exists $a,b\in\mathbb{R}$ such that $x\in(a,b)\subseteq\mathbb{Q}$. However we know that between any two real numbers an irrational number exists. Therefore there exists irrational number $c\in(a,b)$ but $c\notin\mathbb{Q}$. Therefore $(a,b)\nsubseteq\mathbb{Q}$. So $\mathbb{Q}$ is not open.

We show that $\mathbb{R}\backslash\mathbb{Q}$ is not open. We take any $x\in\mathbb{R}\backslash\mathbb{Q}$. Then we know between any two real numbers $a,b$, there exists a rational number. Therefore we cannot make an interval $(a,b)\subseteq\mathbb{R}\backslash\mathbb{Q}$ because there are gaps in the number line. Therefore $\mathbb{Q}$ is not a closed set.

9. The only clopen subsets of $\mathbb{R}$ are $\mathbb{R}$ and $\emptyset$.

