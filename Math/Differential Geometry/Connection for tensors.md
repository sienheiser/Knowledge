#DifferentialGeometry 

We have shown how to fix a connection in [[Requirement to fix a connection| requirement to fix a connection]] and we have shown the same connection coefficients can be used to specify the action of a connection on a covector in [[Connection for covectors| connection for covectors]]. We now specify the action of the connection on a tensor $T$ of rank  $(1,2)$.

Suppose we have given a chart $(U,x)$ on a smooth manifold $M$ where the tensor field $T$ exits. Then
$$
(\nabla_X T)^i_{jk} = X^a\frac{\partial}{\partial x^a}T^i_{jk}+\Gamma^i_{ba}T^b_{jk}X^a-\Gamma^{b}_{ja}T^i_{bk}X^a-\Gamma^{b}_{ka}T^i_{jb}X^a.
$$