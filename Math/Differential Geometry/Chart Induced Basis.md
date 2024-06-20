#DifferentialGeometry
Let $(U,x)\in \mathcal{A_{\text{smooth}}}$, $p\in U$. Suppose we are given set of basis $\frac{\partial}{\partial x^i}$ where $i = 1,2,..., d$ for $T_pM$ (Note that $U\subset M$). Since a chart defines a $d$-coordinate maps lets look at how a vector constructed by the basis acts on a coordinate map $x^j$

$$
\lambda^i(\frac{\partial}{\partial x^i})_p(x^j):= \lambda^i\partial_i(x^j\circ x^{-1})(x(p))
$$

Now  $x^j\circ x^{-1}: \mathbb{R}^d\rightarrow\mathbb{R}$ meaning it takes a tuple $(\alpha_1,...,\alpha_d)$ and returns the $\alpha_j$. ***Therefore, the derivative of the map w.r.t the $i$ th component gives a kronecker delta***. So 
$$
\lambda^i\partial_i(x^j\circ x^{-1})(x(p)) = \lambda^i \delta_i^j = \lambda^j.
$$

However for the basis to be linearly independent we must impose the condition $\lambda^i(\frac{\partial}{\partial x^i})_p = 0$ where the only possible solution is all the $\lambda$'s  equaling zero. Therefore $\lambda^i(\frac{\partial}{\partial x^i})_p x^j = 0\implies \lambda^j = 0$. 

### Note
I have highlighted a sentence, the step where we get the kronecker delta is ambiguous w.r.t to what components are we differentiating. 