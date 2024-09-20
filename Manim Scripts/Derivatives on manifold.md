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

## Velocity Vectors in Euclidean space
In this video we are going to talk about defining velocity vectors of a curve on a manifold. Let us start by looking at how we define velocity vectors of a curve in calculus.

Let us bring in our coordinate system with a plot and place a point on the plot. Now we can define an arrow from the origin of the coordinate to that point with components (1,0). If we move the point along the curve we get the following behaviour. Let us move back to the initial position. 

The curve has the following parametrization. If we take the derivative of this parametrization we get (1,2x) which is the components of our velocity vector. We can bring in our velocity vector and move along the curve.

We want to define the same behaviour on a manifold.

## Velocity Vectors on a Manifold
### Arbitrary manifold
Let us place an arbitrary manifold. On this manifold we have some smooth curve $\gamma$ which can be viewed as a function from the $\mathbb{R}$ to $M$. We can try taking the derivative of this function. The derivative has the following definition so let us pick two points on the curve. We have a problem: on an arbitrary manifold there is no notion of addition between two points so we cannot do this.

### Defining C_infty
Mathematicians use a trick. They make a set called $C^{\infty}(M)$ whose elements are functions  that map from $M$ to $\mathbb{R}$ and are smooth.

### Going from gamma to f of gamma
So let's place $\gamma:\mathbb{R}\rightarrow M$ on the left side and pick some arbitrary smooth function $f:M\rightarrow \mathbb{R}$ on the right side. If we start with a real line on the left side $\gamma$ will take this line and map it to the following curve on the manifold. Then the arbitrary function $f$ will take the curve and map it to a real line. We get the following function $f\circ \gamma$
## Equations


## Circle example
### Introduce circle
Let's look at the example of a circle. If we recollect, a circle is just a set of tuples. If I go around the circle we see the different values these tuples have. Before we compute the velocity vectors on this circle we need derive charts. In my previous video on manifolds I used the circle as an example and made four charts, in this video I would like to derive another set of charts.

We start by drawing a line from point $(1.0,0.0)$ to an arbitrary point $(x,y)$. The slope $s_1$ of this line has form $s_1=\frac{y}{x-1}$. The following line above represents the chart and the point on the circle corresponds to the point on the chart. We can move the point $(x,y)$ around and compute the slope for line. Notice as we approach point $(1,0)$ the slope approached infinity. If we used the slope as a chart the only point we cannot describe on a circle is $(1.0,0.0)$. The solution to this issue is to compute the slope for a second line. Let us go back to our original point. We can draw a second line from point $(-1.0,0.0)$ to the arbitrary point $(x,y)$. The equation of the slope for this line is $s_2=\frac{y}{x+1}$.  The second chart goes to infinity as we approach point $(-1,0)$. We can rename these functions to chi_left and chi_right where left means we use it on the left side of the circle and right means we use it on the right side of the circle.

We can also compute the inverses of these functions they are the following. To derive these expressions you need to use both the charts and the fact that we only input points from a circle.

## Equations
Now that we have defined charts for our circle, let us do some algebra. We start by defining our curve to be $$\gamma(\alpha)=(\cos\alpha,\sin\alpha).$$So this curve just goes around the circle. Next we apply the left chart onto this curve which gives us $$\chi_{\text{l}}\circ\gamma(\alpha) = \frac{\sin\alpha}{\cos\alpha - 1}.$$ Next we take the derivative of this expression which gives us
$$
(\chi_{\text{l}}\circ\gamma)'(\alpha)=-\frac{1}{\cos(\alpha)-1}.
$$
Previously, we had derived the following expression for the derivative on a manifold
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
This term just depends on the chart we choose. Let us try to understand what this equation is telling us. We start by bringing our chart. Then the basis basis vector at a point say 0.79 is the following arrow. If we move along the chart the arrow just stays as the same size. Let us bring our arrow back and make it scale according to the scalar function we have. We get the following behavior. That is it, we have defined velocity vectors on manifolds by using charts and arbitrary smooths functions.


