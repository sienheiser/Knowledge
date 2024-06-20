********
## Definiton

### Vertical Bundle
Let $\pi:E\rightarrow M$ be a smooth fibre bundle.  Then we look at the push-forward of $\pi$ at a point $e\in E$, denoted $\pi_{* e}:T_eE\rightarrow T_{\pi(e)}M$. We define the Vertical tangent space at $e$
$$
V_eE := \text{ker}(\pi_{*e})=\{X\in T_eE|\pi_{*e}(X) = 0\}.
$$
Suppose we have curve $\gamma : \mathbb{R}\rightarrow E$ such that $\gamma(0)= e$, then we have $X_{\gamma,e}\in T_e E$. Now 
$$
\begin{aligned}

\pi_{*e}(X_{\gamma,e})f &= X_{\gamma,e}(f\circ\pi)\\
&= (f\circ\pi\circ\gamma)'(0)\\
&\stackrel{?}{=}0
\end{aligned}
$$
The last equality is only true if $\pi\circ\gamma(\lambda) = constant$ $\forall \lambda\in\mathbb{R}$. This means these tangent vector point along the fibres.

### Ehresmann conneciton

*Definiton:* An Ehresmann connection on a [[Physics/Lectures on Geometrical anatomy on Theoretical physics/Lecture 6/Bundles#Fibre bundle|fibre bundle]] $(E,\pi,M)$ is a smooth subbundle $H$ of $TE$, called the horizontal bundle of the connection, which is complementary to $V$, in the sense that 
$$
TE = H\oplus V.
$$
Furthermore,
1. For each point $e\in E$, $H_e$ is a vector subspace to $T_eE$ at $e$, called the horizontal subspace of the connection at $e$
2. $H_e$ depends smoothly on $e$
3. For each $e$, $H_e \cap V_e = \{0\}$
4. Any tangent vector in $T_eE$ is the sum of a horizontal and vertical component, so that $T_eH=H_e \oplus V_e$.
Where 
$$ 
H_e\oplus V_e = \{\alpha v+\beta h|\alpha,\beta\in\mathbb{R} :v\in V_e:h\in H_e\}.
$$
$$
\begin{align*} X(Y(f)) &= X\left((x^i\circ\sigma)'(\lambda)\frac{\partial}{\partial x^i}_{\sigma(\lambda)}(f)\right) \\ 
&= X\left((x^i\circ\sigma)'(\lambda)\frac{\partial f}{\partial x^i}(\sigma(\lambda))\right) \\ 
 
 &= (x^i\circ\sigma)''(\lambda)X^i(\sigma(\lambda))\frac{\partial f}{\partial x^i}(\sigma(\lambda)) + (x^i\circ\sigma)'(\lambda)\frac{\partial}{\partial x^i}_{\sigma(\lambda)}\left(X^j(\sigma(\lambda))\frac{\partial f}{\partial x^j}(\sigma(\lambda))\right) \end{align*}
$$