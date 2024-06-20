#DifferentialGeometry

We have defined what a connection is [[Connection|here]]. We now look at what it takes to fix a connection $\nabla$. Suppose we have a chart $(U,x)$ and a vector field $X,Y$ exists in reigon $U$ of the smooth manifold $M$. Then we may look at the components of the vector field $\nabla_X Y$
$$
\begin{aligned}
\nabla_XY &= \nabla_{X^i\frac{\partial}{\partial x^i}}(Y^j\frac{\partial}{\partial x^j})\\
&= X^i\left[\nabla_{\frac{\partial}{\partial x^i}}(Y^j)\frac{\partial}{\partial x^j}+Y^j\nabla_{\frac{\partial}{\partial x^i}}(\frac{\partial}{\partial x^j})\right]
\end{aligned}
$$

where in the second equality we have used rules $(iii)$ and $(iv)$ from the definition of a [[Connection|connection]]. To elaborate: $X^i$ and $Y^j$ are just $C^{\infty}(M)$ functions. The term first term $\nabla_{\frac{\partial}{\partial x^i}}(Y^j)\frac{\partial}{\partial x^j}$ just gives another smooth function because of rule $(i)$. The second term $\nabla_{\frac{\partial}{\partial x^i}}(\frac{\partial}{\partial x^j})$ is just another vector field therefore we may write $\nabla_{\frac{\partial}{\partial x^i}}(\frac{\partial}{\partial x^j}) = \Gamma^q_{ji}\frac{\partial}{\partial x^q}$. The final equation we get is 

$$
\nabla_XY = X^i\left[ \nabla_{\frac{\partial}{\partial x^i}}(Y^j)\frac{\partial}{\partial x^j} +  Y^j\Gamma^q_{ji}\frac{\partial}{\partial x^q}  \right].
$$

Therefore to specify the action of a connection we need to specifiy the functions $\Gamma^q_{ji}$ which are completely chart dependent functions.