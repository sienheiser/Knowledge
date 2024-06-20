Suppse we have a smooth manifold $(M,\mathcal{O},\mathcal{A})$, a function $f:M\rightarrow \mathbb{R}$. Choose two charts $(U,x)$ and $(U,y)$ on the same domain. We can define chart transition map $\phi = y\circ x^{-1}$. Then the following 'usual' integral can be done
$$
\begin{aligned}
\int_{y(U)}d^d\beta f_{(y)}(\beta) &= \int_{x(U)}d^d\alpha |det(\partial_a (y^b\circ x^{-1}))(\alpha)|(f_{(y)}\circ y^b\circ x^{-1})(\alpha)\\
&=\int_{x(U)} d^d\alpha |det\frac{\partial y^b}{\partial x^a}| (f\circ y^{-1}\circ y\circ x^{-1})(\alpha)\\
&= \int_{x(U)} d^d\alpha |det\frac{\partial y^b}{\partial x^a}| (f\circ x^{-1})(\alpha)\\
&= \int_{x(U)} d^d\alpha |det\frac{\partial y^b}{\partial x^a}| (f_{(x)})(\alpha)\\
&\neq \int_{x(U)} d^d\alpha f_{(x)}(\alpha)
\end{aligned}
$$

This is not good as we expect to have the same integration form in any chart. But clearly this is not the case with normal integration.