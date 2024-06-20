#DifferentialGeometry
For each point $p\in M$ the tangent space to $M$ at $p$ is 
$$
T_pM := \{\mathcal{v}_{\gamma,p}|\gamma \quad \text{is a smooth curves}\}.
$$

where $\mathcal{v}_{\gamma,p}$ is the [[Velocity|velocity]] of the curve $\gamma$ at point $p$. Take any point $p$ on the manifold. Then imagine any curve that passes throught this point $p$ they belong to the set $T_pM$. 

The tangent space $T_pM$ can be made into a vector space by defining operations like in [[Homomorphsim|homomorphsim]] 
$$
\begin{aligned}
(\mathcal{v}_{\gamma,p} \oplus \mathcal{v}_{\delta,p})(f) :=& \mathcal{v}_{\gamma,p}(f)+_\mathbb{R} \mathcal{v}_{\delta,p} (f)\\
(\alpha\odot \mathcal{v}_{\gamma,p})(f) :=& \alpha\cdot_\mathbb{R}\mathcal{v}_{\gamma,p}(f)\\
\end{aligned}
$$
where $f$ is an arbitrary smooth function.

We need to still show that the tangent vector space is closed under the defined addition and s-multiplication. The proof for this is shown [[Proof that Tangent Vector Space is closed|proof]].