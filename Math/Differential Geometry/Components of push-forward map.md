Suppose we have two charts $(U,x)\in M$ and $(V,y)\in M$ where $M$ and $N$ are two different differetiable manifolds. Let us have a [[Push-forward map|push-forward map]] that takes vectors from [[Tangent Bundle of a Smooth Manifold|tangent bundle]] $TM$ to tangent bundle $TN$. Then the components of the push forward map can be found by 

$$
\begin{aligned}
dy^a(\phi_*(\frac{\partial}{\partial x^i})_p) &\equiv\phi_*(\frac{\partial}{\partial x^i})_py^a\\
&\equiv \frac{\partial}{\partial x^i}_p(y\circ \phi)^a\\
&\equiv \frac{\partial \hat{\phi}^a}{\partial x^i}
\end{aligned}
$$
where the first definiton is $df(X) \equiv Xf$ the second definition comes from the definition of the [[Push-forward map|push-forward map]] and the final definiton is our new definition. Note the $a$ indicied live in the $N$ manifold while the $i$ indicies live in the $M$ manifold. 