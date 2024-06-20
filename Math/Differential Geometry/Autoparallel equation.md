When we say autoparallel we mean [[Autoparallely transported curves|auto parallelity transported]]. Given smooth manifold with connection$(M,\mathcal{O},\mathcal{A},\nabla)$. Suppose we have chart $(U,x)$ where a part of smooth curve $\gamma:\mathbb{R}\rightarrow M$ passes through. Then
$$
\begin{aligned}
\nabla_{\mathcal{v}_\gamma}\mathcal{v}_\gamma \iff & \dot{\gamma}^i\frac{\partial}{\partial x^i}(\dot{\gamma}^q)+\Gamma^q_{ji}\dot{\gamma}^i\dot{\gamma}^j = 0\\
\implies & \ddot{\gamma}^q +\Gamma^q_{ji}\dot{\gamma}^i\dot{\gamma}^j = 0\\
\iff & \ddot{\gamma}_{(x)}^q(\lambda)+\Gamma^q_{(x)ji}(\gamma(\lambda))\dot{\gamma}_{(x)}^i(\lambda)\dot{\gamma}_{(x)}^j(\lambda) = 0
\end{aligned}
$$
where we are looking at the $q$ th component in the chart $x$. To see that $\dot{\gamma}^i\frac{\partial\dot{\gamma}^q}{\partial x^i} = \ddot{\gamma}$ use the definition in [[Components of a vector w.r.t a chart]]. So 
$$
\begin{aligned}
\dot{\gamma}^i\frac{\partial\dot{\gamma}^q}{\partial x^i} &:= (x\circ \gamma)^{'i}\partial_i(\dot{\gamma}^q\circ x^{-1})\\
&= ((\dot{\gamma}^q\circ x^{-1})\circ(x\circ\gamma))'\\
&= (\dot{\gamma}^q\circ\gamma)'\\
&= ((x\circ\gamma)^q{}'\circ \gamma)'
\end{aligned}
$$
so we see that this the taking a $\lambda$ as the input taking the first derative then taking the second derivative w.r.t to the $q$th component.

### Example
Suppose we have $(S^2,\mathcal{O},\mathcal{A},\nabla_{round})$ consider a chart that takes a point $p\in M$ and maps it as such $x(p) = (\theta,\phi)$. The only non zero connection coefficients are 
$$
\begin{aligned}

\Gamma_{(x)22}^1(x^{-1}(\theta,\phi)) &= -\sin(\theta)\cos(\theta)\\
\Gamma_{(x)21}^2(x^{-1}(\theta,\phi)) &= \Gamma_{(x)12}^2(x^{-1}(\theta,\phi)) = \cot(\theta)

\end{aligned}
$$

Then the autoparallel equations we get are 

$$
\begin{aligned}
\ddot{\theta}+\Gamma_{22}^1\dot{\phi}\dot{\phi} &= 0\\
\ddot{\phi}+2\Gamma_{12}^2\dot{\theta}\dot{\phi}&=0

\end{aligned}
$$

At the equator of the sphere with $\theta = \pi/2$ we get $\phi(\lambda) = \omega\lambda+\phi_0$.