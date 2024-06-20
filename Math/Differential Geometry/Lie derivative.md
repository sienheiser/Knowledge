The Lie derivative makes checking for symmetry child's play.
*Definition:* If $\forall X\in L$ where $L$ is a lie algebra
$$
\mathcal{L}_xg:= \lim_{\lambda\rightarrow 0}\frac{(h^*_\lambda)^*g-g}{\lambda} = 0
$$
where $(h^*_\lambda)^*$ can be viewed as a [[Pull back map|pull back map]]. Then $L$ is a symmetry of $g$.

*Definition:* The Lie derivative $\mathcal{L}$ on a smooth manifold $(M,\mathcal{O},\mathcal{A})$ sends a pair of a vector field $X$ and a $(p,g)-$tensor field $T$ to a $(p,q)$-tensor field such that 

1. $\mathcal{L}_Xf = X(f)\quad \forall f\in C^{\infty}(M)$
2. $\mathcal{L}_X Y = [X,Y]\quad Y\text{ is a vector field}$
3. $\mathcal{L}_X(T+S) = \mathcal{L}_XT+\mathcal{L}_xS$
4. $\mathcal{L}_X(T(\omega,Y)) = \mathcal{L}_X(T(\omega,Y))+T(\mathcal{L}_X(\omega),Y)+T(\omega,\mathcal{L}_X(Y))$
5. $\mathcal{L}_{X+Y}T = \mathcal{L}_X T+\mathcal{L}_YT$

in axiom 4 we only show Leibiniz rule for (1,1) tensor field. But can be generalized to arbitrary tensor field.