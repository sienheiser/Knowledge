Properties for [[Lebegue integration]] for [[Measureable non-negative functions|measureable non-negative functions]] $f,g$. 
1. Markov inequality: For $z\in\mathbb{R}^+_0$ $$\int fd\mu\geq z\cdot\mu(\text{preim}_f(\{z\}).$$
2. $f\leq_{\text{a.e}}g\implies \int fd\mu\leq\int gd\mu$.
3. $f =_{\text{a.e}}g\implies \int fd\mu=\int gd\mu$.
4. $\int fd\mu = 0 \implies f =_{\text{a.e}}0.$
5. $\int f d\mu < \infty \implies f <_{\text{a.e}} \infty.$

where $a.e.$ is true [[A set of measure zero|almost everywhere]].

*Thoerem on monotone convergence:* Let $0\leq f_1\leq f_2\leq...\leq f_n$ be a sequence of [[Measureable maps|measureable functoins]] $f_n:M\rightarrow \overline{R}$. Provided $f:=\sup_{n\geq 1}  f_n$ with point wise convergence then 
$$
\lim_{n\rightarrow \infty}\int f_nd\mu = \int fd\mu.
$$

Theorem: Let $f,g\geq 0$ be measureable. Let $\alpha \in \mathbb{R}_0^+$. Then
$$
\int (f+\alpha g)d\mu = \int fd\mu+\alpha\int gd\mu.
$$

Theorem: For any sequence $f_n:M\rightarrow \overline{\mathbb{R}}_0^+$ of measureable functions we have
$$
\int (\sum_{n=1}^\infty f_n)d\mu = \sum_{n=1}^\infty\int f_nd\mu.
$$