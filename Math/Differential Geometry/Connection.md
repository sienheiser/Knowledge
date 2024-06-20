#DifferentialGeometry

We have talked a bit about notation [[Directional derivative notation|here]]. We now define what a directional derivative/connection is on a manifold.

*Definiton*: A connection $\nabla$ on a smooth manifold $(M,\mathcal{O},\mathcal{A})$ is a map that takes a vector (field) and a (p,q)-tensor (field) $\mathbb{T}$ and sends them to a (p,q)-tensor (field) $\nabla_X\mathbb{T}$. The connection satifies the following 

$$
\begin{aligned}
(i)&\quad\nabla_X f = Xf\\
(ii)&\quad \nabla_X (T+S) = \nabla_X T+ \nabla_X S\\
(iii)&\quad \nabla_X (T(\omega,Y)) = \nabla_X T(\omega,Y)+T(\nabla_X \omega,Y)+T(\omega,\nabla_X Y)\\
(iv)& \quad \nabla_{(fX+Z)}T = \nabla_{fX}T+\nabla_Z = f\nabla_X T+ \nabla_Z T.
\end{aligned}
$$
*Remark*: $f\in C^{\infty}(M)$ in (i) and (iv). The tensor in (iii) is of rank (1,1). The rule can be generalized to an arbitrary (p,q)-tensor. All vector field $X,Z\in \Gamma(TM)$.

*Definition:* A manifold with connection is a quadruple $(M,\mathcal{O},\mathcal{A},\nabla)$. 
