Let $f,g$ be integrable functions $M\rightarrow \mathbb{R}$. Then
1. $f\leq_{\text{a.e}}g\implies \int fd\mu\leq\int gd\mu$
2. $\forall \alpha\in\mathbb{R}$ we have $$\int (f+\alpha g)d\mu = \int fd\mu+\alpha\int gd\mu.$$

*Theorem on dominant convergence:*
Let 
1. $f_1,f_2,...$ be a sequence of [[Measureable maps|measureable]] functions.
2. Let $f_n\rightarrow_{\text{a.e}}f$ pointswise for some $f$.
3. Let $g$  be a [[Measureable non-negative functions|measureable non-negative functions]] with $\int gd\mu < \infty$ such that $\forall n\in\mathbb{N}\quad |f_n|\leq_{\text{a.e}}g$.

Then we have

1. $f$ and $f_1,f_2,...$ are integrable
2. $\lim_{n\rightarrow\infty}\int |f_n-f|d\mu = 0$
3. $\lim_{n\rightarrow\infty}f_nd\mu = \int fd\mu$

Finally we have *Markov identity*
$$
\forall z\in\mathbb{R}_0^+:\int fd\mu\geq z\cdot\mu(\text{preim}_f([z,\infty))).
$$