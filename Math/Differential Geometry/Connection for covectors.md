#DifferentialGeometry

In [[Requirement to fix a connection|requirement to fix a connection]] we showed that if we fix the connection coefficients $\Gamma_{ij}^q$ for a chart then we can compute the action of a connection on a vector field. Can we use the same connection coefficients to look at the action of a connection on a covector? Suppose we take 
$$
\nabla_{\frac{\partial}{\partial x^j}} dx^i = \Sigma^i_{mj}dx^m.
$$

Then look at 
$$
\nabla_{\frac{\partial}{\partial x^m}}\left(dx^i(\frac{\partial}{\partial x^j})\right) = \nabla_{\frac{\partial}{\partial x^m}}\left(\delta^i_j\right) = 0.
$$

But using the Leibiniz rule we can also do

$$
\begin{aligned}
\nabla_{\frac{\partial}{\partial x^m}}\left(dx^i(\frac{\partial}{\partial x^j})\right) &= \left(\nabla_{\frac{\partial}{\partial x^m}}(dx^i)\right)\frac{\partial}{\partial x^j} + dx^i \nabla_{\frac{\partial}{\partial x^m}}(\frac{\partial}{\partial x^j})\\
&= \Sigma^i_{km}dx^k(\frac{\partial}{\partial x^j})+dx^i\Gamma_{jm}^{q}\frac{\partial}{\partial x^q}\\
&= \Sigma^i_{jm}+\Gamma^i_{jm}.
\end{aligned}
$$

We know that 
$$
\Sigma^i_{jm}+\Gamma^i_{jm} = 0 \implies \Sigma^i_{jm} = -\Gamma^i_{jm}
$$

So we may use the same connection coefficients to specify the actions of a connection on a covector.