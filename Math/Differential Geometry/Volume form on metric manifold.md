On a  $(M,\mathcal{O},\mathcal{A},g)$  metric manifold one can construct volume form $\Omega$ from $g$ in any chart as
$$
\Omega_{(x)i_1,...,i_d} := \sqrt{\text{det}(g_{(x)ij})}\epsilon_{i_1,...,i_d}
$$
where $\epsilon_{i_1,...,i_d}$ is the Levi-Civita symbol.

Transformation of this form is well defined. Proof
$$
\begin{aligned}
\Omega_{(y)i_1,...,i_d} &:= \sqrt{\text{det}(g_{(y)ij})}\epsilon_{i_1,...,i_d}\\
&=\sqrt{\text{det}(g_{(x)mn})\frac{\partial x^m}{\partial y^i}\frac{\partial x^n}{\partial y^j}}\text{det}\left(\frac{\partial y}{\partial x}\right)\epsilon_{i_1,...,i_d}\\
&=\sqrt{\text{det}(g_{(x)mn})}\left|\frac{\partial x}{\partial y}\right|\text{det}\left(\frac{\partial y}{\partial x}\right)\epsilon_{i_1,...,i_d}\\
&= \sqrt{\text{det}(g_{(x)mn})}\text{sgn}\left(\frac{\partial x}{\partial y}\right)\epsilon_{i_1,...,i_d}\\.
\end{aligned}
$$
Therefore $\Omega$ is well defined iff $\text{det}(\frac{\partial y}{\partial x})>0$ for any pair of charts $(U,x)$ and $(U,y)$. Therefore we further restrict our atlas to something called an oriented atlas denoted $\mathcal{A}^{\uparrow}$ where the sign of the determinant is always positive.