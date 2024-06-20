---
aliases: [projecting functions]
---

#math

Suppose we have an interval $\Lambda = [x_{min},x_{max}]$ where $x_{min}$ and $x_{max}$ are real numbers. If we want to create a [[vector space]] with [[basis]] we need to define a [[scalar product]] on $\Lambda$. If $w$ is a positive function on $\Lambda$, the scalar product between two functions $f$ and $g$ w.r.t the [[Math/MeasureTheory/measure]] $w$ can be defined as 

$$
(f,g)_w = \int_\Lambda f(x)g(x)w(x)dx. 
$$

Using this scalar product an orthnormal set of polynomials upto degree $N$ can be found for the polynomial vector space $\mathbb{P}^N$. To project any function $u$ in this space we simply use the following procedure

$$
u = \sum_{n = 1}^N \hat{u}_n p_n(x)
$$
where $\hat{u}=\frac{(u,p_n)}{(p_n,p_n)}$. 
