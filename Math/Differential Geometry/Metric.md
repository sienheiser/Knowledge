We want structure that defines length and angle between vectors at each tangent vector $T_pM$ in a manifold. 

*Definition:* A metric $g$ on a smooth mfd $(M,\mathcal{O},\mathcal{A}$ is a (0,2)-tensor field satisfying
1.	symmetric: g(X,Y) = g(Y,X)
2.	non-degeneracy: the musical map ''flat'' $\flat:\Gamma(TM)\rightarrow \Gamma(TM)$ is defined as
$$
\begin{aligned}
X\rightarrow \flat(X)\\
\flat(X)(Y)&:= g(X,Y)
\end{aligned}
$$
   and the flat map needs to be an isomorphism meaning it is invertible.


*Definiton*: The (2,0)-tensor filed $g^{'-1'}$ w.r.t to a metric g is the symmetric map 
$$
\begin{aligned}
g^{'-1'}:\Gamma(T^*M)\times\Gamma( T^*M)&\tilde{\rightarrow} C^{\infty}(M)\\
(\omega,\sigma)\rightarrow \omega(\flat^{-1}(\sigma))

\end{aligned}
$$

In a chart $g_{ab}g^{bc} = \delta_a^c$ so it seems to be an inverse but really it is not an inverse.