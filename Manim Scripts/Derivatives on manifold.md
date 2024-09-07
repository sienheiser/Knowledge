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

## Circle example
### Introduce circle
Let's look at the example of the circle. If we recollect a circle is just a set of tuples. If I go around the circle we see the different values these tuples have. But first let us derive our charts  for the circle. In my previous video on manifolds I used the circle as an example and made four charts, in this video I would like to derive another set of charts.

We start by drawing a line from point $(1.0,0.0)$ to  an arbitrary point $(x,y)$. We can move the point $(x,y)$ around and compute the slope for line. Notice as we approach point $(x,y)$ the slope approached infinity. If we used