In this note we will show how compute left invariants fields given a Lie groups $G$. We do this by first defining the left map $\forall g\in G|l_g:G\rightarrow G$. Then we use the fact that Lie groups are differential manifolds that come with charts. By using these charts we compute the left invariant fields.

## Left map
*Definition:* $\forall g\in G$ the map
	$$l_g:G\rightarrow G$$
is defined as $l_g(h)=g\cdot h$. We call $l_g$ the left map.

## Computing left invariant fields
Suppose $G$ is a $n$-dimensional manifold. Let $(x,U)$, where $U$ is an open subset of $G$ that contains the identity, be the chart we use to compute the left invariant fields. We start by looking at expression 
$$
l_{a*}(X_e)f
$$
where $l_{a*}$ is the push-forward map of $l_a$, $X_e$ is a tangent vector at the identity of $G$ and $f$ is a smooth function from $G$ to $G$. This expression essentially takes the tangent vector $X_e$ pushes it forward to the point $a$. We may compute what is the resulting vector by first computing the action $l_{a*}$ on the basis vectors produced by the chart. Therefore we look at 
$$
\begin{aligned}
l_{a*}\left(\frac{\partial}{\partial x^l}\right)&\stackrel{1}{=} \left(\frac{\partial}{\partial x^l}\right)_e(f\circ l_a)\\
&\stackrel{2}{=}\partial_l(f\circ l_a\circ x^{-1})(x(e))\\
&\stackrel{3}{=}\partial_l(f\circ x^{-1}\circ x\circ l_a\circ x^{-1})(x(e))\\
&\stackrel{4}{=}\partial_l(x\circ l_a\circ x^{-1})^m(x(e))\partial_m(f\circ x^{-1})(x(a))\\
&\stackrel{5}{=} \partial_l(x\circ l_a\circ x^{-1})^m(x(e))\left(\frac{\partial}{\partial x^m}\right)_a f.
\end{aligned}
$$
 where $\stackrel{1}{=}$ is true because of the definiton of [[Push-forward map]], $\stackrel{2}{=}$ is true because of the definiton of $(\frac{\partial}{\partial x^1}) f$, $\stackrel{3}{=}$ is true because we just inlude the identity map, $\stackrel{4}{=}$ is true because associativity of composition between maps and we took the derivatives and $\stackrel{5}{=}$ is true because of the same reason as $\stackrel{3}{=}$. 

To get the components we have to first compute what 
$$
x\circ l_a\circ x^{-1}(x(b_1,...,b_n))
$$
is. Then we take the dervative w.r.t to the $l$ index. In this way we have constructed our left invariant fields after inputing our results back.
