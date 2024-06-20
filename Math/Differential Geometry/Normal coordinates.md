#DifferentialGeometry 

*Definition:* Let $p\in M$ of $(M,\mathcal{O},\mathcal{A},\nabla)$. Then one can construct a chart $(U,x)$ where $p\in U$ such that 
$$
\Gamma^{i}_{(x)jk}(p) = 0
$$
at the point $p$. Not neccessary in any neighbourhood.

Proof: Let $(V,y)$ be any chart $p\in V$. Thus in general $\Gamma_{(y)(jk)}^i \neq 0$ at $p$ where we have considered the symmetric part of the connection coefficients. Then consider a new chart $(U,x)$ to which one transits by virtue of 
$$
(x\circ y^{-1})^i(\alpha^1,...,\alpha^d):=\alpha^i\pm\Gamma^i_{(y)(mk)}\alpha^m\alpha^k 
$$
where we have defined the action of the chart on a tuple of coordinates. Note that we place $\Gamma_{(y)(mk)}^i$ from the y-chart not a mistake. Then we take the first derivative w.r.t to $y^j$ 
$$
\frac{\partial (x\circ y^{-1})^i}{\partial y^j}:= \frac{\partial x^i}{\partial y^j} = \delta^i_j\pm \Gamma^i_{(y)(jk)}\alpha^k 
$$
then take a second derivative

$$
\frac{\partial^2 x^i}{\partial y^l \partial y^j} = \Gamma^i_{(y)(lj)} 
$$

Then using the change of connection formula we have

$$
\begin{aligned}
\Gamma^i_{(x) (jk)}(p) &= \Gamma_{(y) jk}^i(p) - \Gamma_{(y)(kj)}^i(p)\\
&= \Gamma_{(y)[jk]}^i(p) 
\end{aligned}
$$

where the last term is known as the torsion tensor.