Suppose we have two manifolds $M$ and $N$ with a map $\phi$ taking points from $M$ and mapping them to $N$.
Suppose we have curve $\gamma:\mathbb{R}\rightarrow M$  then we can define the tangent vectors of the curve $\mathcal{v}_{\gamma,p}$ at a point $p$. We claim that if we map the curve $\gamma$  to $N$ using $\phi\circ\gamma$ then the tangent vectors of curve $\phi\circ\gamma$ is $\phi_*(\mathcal{v}_{\phi\circ\gamma,\phi(p)})$.

Proof: Given $f\in C^{\infty}(N)$ and $\gamma(\lambda_0) = p$. Then
$$
\begin{aligned}
\phi_*(\mathcal{v}_{\gamma,p})f&\equiv  \mathcal{v}_{\gamma,p}(f\circ\phi)\\
&\equiv (f\circ\phi\circ\gamma)'(\lambda_0)\\
&= \mathcal{v}_{\phi\circ\gamma,\phi(p)}f

\end{aligned}
$$