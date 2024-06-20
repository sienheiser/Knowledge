Suppose we have two metric manifolds $M$ and $N$. Let $dimM < dimN$ and let $\phi:M\rightarrow N$ be an injective map. Suppose we know the metric $g$ in $N$. Can we induce a metric in $M$ using the metric $g$. Yes! Take two vectors $X$ and $Y$ belonging to $M$. Then
$$
\begin{aligned}

&g_M(X,Y)\equiv g(\phi_*(X),\phi_*(Y))\\
&\implies (g_M)_{ij} = g_{ab}(\frac{\partial\hat{\phi}^a}{\partial x^i})_{\phi(p)}(\frac{\partial \hat{\phi}^b}{\partial x^j})_{\phi(p)}
\end{aligned}
$$