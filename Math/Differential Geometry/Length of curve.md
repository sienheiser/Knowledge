Let $\gamma$ be a smooth curve. Then we know is [[Velocity|velocity]] $\mathcal{v}_{\gamma,\gamma(\lambda)}$ at each $\gamma(\lambda)\in M$.

*Definiton:* On a Riemmanian metric manifold $(M,\mathcal{O},\mathcal{A},g)$ the speed of a curve at $\gamma(\lambda)$ is the number 
$$
\sqrt{g(\mathcal{v}_{\gamma,\gamma(\lambda)},\mathcal{v}_{\gamma,\gamma(\lambda)})} = s(\lambda)
$$


*Definiton:* Let $\gamma:(0,1)\rightarrow M$ be a smooth curve. Then the length of $\gamma$ is the number
$$
L[\gamma] := \int_0^1 d\lambda \sqrt{g(\mathcal{v}_{\gamma,\gamma(\lambda)},\mathcal{v}_{\gamma,\gamma(\lambda)})}
$$


### Example

Suppose  on a 2D  metric manifold we are given metric $g_{00} = R^2$ and $g_{11} = R^2\sin{\theta}$. This is the metric of sphere. We may compute the length of the curve at around the equator. Let $\theta(\lambda) = \pi/2$ and $\phi(\lambda)=2\pi\lambda^2$ Then $\theta' = 0$ and $\phi' = 6\pi\lambda^2$. Then the length of the curve
is 

$$
\begin{aligned}
L[\gamma] &= \int^1_0d\lambda \sqrt{R^2\cdot 0+R^2\sin^2(\frac{\pi}{2})\cdot 36\pi^2\lambda^4}\\
&= 6\pi R\int_0^1d\lambda \lambda^2\\
&= 2\pi R
\end{aligned}
$$

### Theorem 

If $\gamma:(0,1)\rightarrow M$ is a smooth curve and $\sigma:(0,1)\rightarrow (0,1)$ is bijective and increasing map then 
$$
L[\gamma] = L[\gamma\circ \sigma].
$$

