#DifferentialGeometry
Let us have a chart $(U,x)\in \mathcal{A}_{\text{smooth}}$. Let $\gamma:\mathbb{R}\rightarrow U$ and $\gamma(0) = p$. Then the [[Velocity|velocity]] is of the curve $\gamma$ at $p$ is 
$$
\begin{aligned}
\mathcal{v}_{\gamma,p} &:= (f\circ \gamma)'(0)\\
&= (f\circ x^{-1}\circ x\circ \gamma)'(0)\\
&= \frac{\partial(f\circ x^{-1})}{\partial(x\circ \gamma)^i}|_{(x\circ \gamma) = x(p)}\frac{d(x\circ \gamma)^i}{d\lambda}|_{\lambda = 0}\\
&= \partial_i(f\circ x^{-1})(x(p))(x\circ \gamma)^{i'} (0).
\end{aligned}
$$

We define 
$$
\begin{aligned}
\partial_i(f\circ x^{-1})(x(p))&:= (\frac{\partial f}{\partial x^i})_p\\
(x\circ \gamma)^{i'} (0) &:= \dot{\gamma}_x^i(0)
\end{aligned}
$$
which gives 
$$
\partial_i(f\circ x^{-1})(x(p))(x\circ \gamma)^{i'} (0) = \dot{\gamma}_x^i(0) (\frac{\partial }{\partial x^i})_p f.
$$
Since $f$ is arbitrary we can take it away and the formula will remain true. We see that the 'partial derivaties' behave as basis, but really we just define the notation. 