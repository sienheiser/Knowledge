## Charts scene

$$\frac{\text{d}}{\text{d}\lambda}(f\circ\gamma)(\alpha):= (f\circ \gamma)'(\alpha)$$
Let $\gamma(\alpha)=p$ 

equation 1
$$
\begin{aligned}
(f\circ\gamma)'(\alpha) &= (f\circ x^{-1}\circ x\circ\gamma)'(\alpha)\\
&= ((f\circ x^{-1})\circ (x\circ\gamma))'(\alpha)\\
&= \partial_i(f\circ x^{-1})(x(p))\cdot(x\circ \gamma)^{\prime i}(\alpha)\\
&=(x\circ \gamma)^{\prime i}(\alpha)\cdot\partial_i(f\circ x^{-1})(x(p))\\
&=(x\circ \gamma)^{\prime i}(\alpha)\cdot \big(\frac{\partial}{\partial x^i}\big )_{\gamma(\alpha)} f
\end{aligned}
$$

Since $f$ is arbitrary we can drop it which gives
$$
(\_\circ\gamma)'(\alpha) = (x\circ \gamma)^{\prime i}(\alpha)\cdot \big(\frac{\partial}{\partial x^i}\big )_{\gamma(\alpha)} \_
$$

