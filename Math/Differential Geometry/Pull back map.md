Suppose we have map $\phi:M\rightarrow N$ where $M$ and $N$ are two differentiable manifolds. Then the pull back map denoted $\phi^*$ is defined as 
$$
\begin{aligned}
\phi^*:&T^*N\rightarrow T^*M\\
&\omega \mapsto \phi^*(\omega)\\
\text{where }&\phi^*(\omega)(X)\equiv \omega(\phi_*(X))
\end{aligned}
$$
where $\phi_*$ is the [[Push-forward map|push forward map]].

Components of pull back map w.r.t charts $(U,x)\in\mathcal{A}_M$ and $(V,y)\in\mathcal{A}_N$ is
$$
\begin{aligned}

\phi^*(dy^a_{\phi(p)})(\frac{\partial}{\partial x^i}) &\equiv dy^a(\phi_*(\frac{\partial}{\partial x^i}_p))\\
&\equiv \frac{\partial \hat{\phi}^a}{\partial x^i}

\end{aligned}
$$
For the definition in the last line see [[Components of push-forward map|components of push-forward map]]. So given two charts in two different manifolds. The components of the push forward and pull back maps are the same.