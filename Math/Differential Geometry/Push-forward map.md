#DifferentialGeometry 
Suppose we have two [[Differentiable Manifold|differentiable manifolds]] $M$ and $N$. Suppose we have map 

$$
M\xrightarrow[]{\phi}N
$$
The above is a [[Math/Differential Geometry/Bundles|bundle]] if $\phi$ is a surjective map.

*Definition:* The push-forward $\phi_*$ is the map 
$$
TM \xrightarrow[]{\phi_*} TN
$$
where 
$$
\begin{aligned}
M \ni X \mapsto \phi_*(X)
\end{aligned}
$$
where $\phi_*(X)f := X(f\circ \phi)$ for any $f\in C^{\infty}(N)$. Something weird with this definition how does $X$ which is an element of $M$ act on a function which belongs to $N$?

