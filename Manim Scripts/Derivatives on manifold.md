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
Let's look at the example of a circle. If we recollect, a circle is just a set of tuples. If I go around the circle we see the different values these tuples have. Before we compute the velocity vectors on this circle we need derive charts. In my previous video on manifolds I used the circle as an example and made four charts, in this video I would like to derive another set of charts.

We start by drawing a line from point $(1.0,0.0)$ to an arbitrary point $(x,y)$. The slope $s_1$ of this line has form $s_1=\frac{y}{x-1}$. We can move the point $(x,y)$ around and compute the slope for line. Notice as we approach point $(1,0)$ the slope approached infinity. If we used the slope as a chart the only point we cannot describe on a circle is $(1.0,0.0)$. The solution to this issue is to compute the slope for a second line. Let us go back to our original point. We can draw a second line from point $(-1.0,0.0)$ to the arbitrary point $(x,y)$. The equation of the slope for this line is $s_2=\frac{y}{x+1}$.  The second chart goes to infinity as we approach point $(-1,0)$. We can rename these functions to chi_left and chi_right where left means we use it on the left side of the circle and right means we use it on the right side of the circle.

We can also compute the inverses of these functions they are the following. To derive these expressions you need to use both the charts and the fact that we only input points from a circle.

## Equations
Now that we have defined charts for our circle, let us do some algebra. We start be defining our curve to be $$\gamma(\alpha)=(\cos\alpha,\sin\alpha).$$So this curve just goes around the circle. Next we apply the left chart onto this curve which gives us $$\chi_{\text{l}}\circ\gamma(\alpha) = \frac{\sin\alpha}{\cos\alpha - 1}.$$ Next we take the derivative of the above which gives us
$$
(\chi_{\text{l}}\circ\gamma)'(\alpha)=-\frac{1}{\cos(\alpha)-1}.
$$
We had derived the following expression for the derivative on a manifold
$$
(\_\circ\gamma)'(\alpha) = (x\circ \gamma)i'(\alpha)\cdot \big(\frac{\partial}{\partial x^i}\big )_{\gamma(\alpha)} \_.
$$
where $\_$ represents an arbitrary smooth function and $x$ is an arbitrary chart.
If we use our left chart we get
$$
(\_\circ\gamma)'(\alpha) = (\chi_{\text{l}}\circ \gamma)'(\alpha)\cdot \big(\frac{\partial}{\partial \chi_{\text{l}}}\big )_{\gamma(\alpha)} \_.
$$
We can then substitute the derivative to get the following
$$
(\_\circ\gamma)'(\alpha) = -\frac{1}{\cos(\alpha)-1}\cdot \big(\frac{\partial}{\partial \chi_{\text{l}}}\big )_{\gamma(\alpha)} \_.
$$
Let try to understand what this means. The $$-\frac{1}{\cos\alpha-1}$$ is just a scalar quantity it depends on the choice of curve $\gamma$ and chart. What about the term $$\frac{\partial}{\partial\chi_{\text{l}}}$$
This term just depends on the chart we choose. Let us try to understand what this equation is telling us.


