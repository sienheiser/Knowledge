#DifferentialGeometry
Let $(U,x)$ and $(V,y)$ be two overlapping charts. Take $p\in U\cap V$. Let $X\in T_pM$ then
$$
X = X_{(x)}^i\frac{\partial}{\partial x^i} = X_{(y)}^j\frac{\partial}{\partial y^j}.
$$

To study the change of components
$$
\begin{aligned}
(\frac{\partial}{\partial x^i})f &:= \partial_i(f\circ x^{-1})(x(p))\\
&= \partial_i((f\circ y^{-1})\circ (y\circ x^{-1}))(x(p))\\
&= \frac{\partial \left((f\circ y^{-1})\circ (y\circ x^{-1})\right)}{\partial (x\circ X)^i}\\
&= \frac{\partial(f\circ y^{-1})}{\partial(y\circ x^{-1})^j}|_{y(p)}\frac{\partial(y\circ x^{-1})^j}{\partial(x\circ X)^i}|_{x(p)}\\
&:= \left(\frac{\partial y^j}{\partial x^i}\right)_p \left( \frac{\partial f}{\partial y^j}\right)_p.
\end{aligned}
$$

The 4th equality is my own way of looking at the derivatives, it does not seem correct but it always leads to the right answer.  Finally we get the following transformation rule

$$
\begin{aligned}
&X^i_{(x)}\left( \frac{\partial}{\partial x^i}\right)_p\\
&= X^i_{(x)}\left(\frac{\partial y^j}{\partial x^i}\right)_p \left( \frac{\partial }{\partial y^j}\right)_p\\
&\implies X^j_{(y)} = X^i_{(x)}\left(\frac{\partial y^j}{\partial x^i}\right)_p.
\end{aligned}
$$
