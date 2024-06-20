#DifferentialGeometry
Let $(M,\mathcal{O},\mathcal{A})$ be a smooth manifold (this will be our base space of the [[Math/Differential Geometry/Bundles|bundle]]). Our goal is to build a bundle using information from the given smooth manifold $(M,\mathcal{O},\mathcal{A})$ and a projection map.

(a) We define a set $TM$ as 

$$
TM:= \bigcup_{p\in M} T_pM
$$
where we still keep the information of which tangent spaces belong to which point. 

(b) To make a [[Math/Differential Geometry/Bundles|bundle]] we define a projection map $\pi$ between $TM$ and $M$. So $TM\xrightarrow[]{\pi}M$. To make it clear $\pi$ takes and element $X\in TM$ which is a vector and maps to a point unique $p$ where we know $X$ should belong to i.e. $X\in T_pM$.

So far we have constructed a set $TM$, a smooth manifold $M$ and a projection $\pi$ from set $TM$ to smooth manifold $M$. We need to make $TM$ a smooth manifold to get a bundle.

(c) We construct [[Coarsest topology|coarsest topology]] for $TM$

(d) We construct atlas for $TM$ from given atlas for $M$ and show that the constucted atlas for $TM$ is smooth [[Constructing Atlas|here]].

Therefore we have a smooth manifold $TM$ so we have finally constructed out tangent bundle of a smooth manifold.

