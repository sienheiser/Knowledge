Let $X_1,...,X_s$ be $s$ many vector fields on $M$, such that 
$$
[X_i,X_j] = C^k_{ij}X_k
$$
where $i,j,k = 1,...,s$ and $C^k_{ij}$ are known as structure constants. The Lie subalgebra is deonted ($\text{span}\{X_1,...,X_s\},[\cdot,\cdot])$.

### Example SO(3) on $S^2$
There are three vector fields with the following symmetry
$$
\begin{aligned}

&[X_1,X_2] = X_3\\
&[X_2,X_3] = X_1\\
&[X_3,X_1] = X_2\\
\end{aligned}
$$
Therefore $(\text{span}\{X_1,X_2,X_3\},[\cdot,\cdot]) = SO(3)$.
Explicitly
$$
\begin{aligned}
X_{1(p)} &= -\sin(\phi(p))\frac{\partial}{\partial \theta}-\cot(\theta(p))\cos(\phi(p))\frac{\partial}{\partial \phi}\\
X_{2(p)} &= \cos(\phi(p))\frac{\partial}{\partial\theta}-\cot(\theta(p))\sin(\phi(p))\frac{\partial}{\partial \phi}\\
X_{3(p)} &= \frac{\partial}{\partial\phi}

\end{aligned}
$$
On a smooth manifold $(S^2,\mathcal{O}_{Standard},\mathcal{A})$ Lie subalgebras can be found.