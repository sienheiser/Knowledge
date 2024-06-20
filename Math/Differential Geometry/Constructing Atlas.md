#DifferentialGeometry
Next question: Is $(TM,\mathcal{O}_{TM})$ a topological manifold.  We need to construct a $C^{\infty}$-atlas on $TM$ from the  atlas $\mathcal{A}$ on $M$. We can define the altas of $TM$ as follows
![[Atlas from M.png]]
In the above picture we consider a subset $u$ of points from base space $M$. We know that chart $(u,x)$ exists and we can map this set of points to a 1D space. However, if we consider the [[Fiber|fibers]] of $u$ (labeled $Tu$ in the figure) then can we build chart for those fibers? We can if we take the follwing definiton of the atlas of $TM$
$$
\mathcal{A}_{TM} = \{ (Tu,\xi_x)|(u,x)\in\mathcal{A}\}
$$
where 
$$
\begin{aligned}
\xi_x:= &Tu\rightarrow \mathbb{R}^{2\cdot dim(M)}\\

&X\rightarrow \left((x^1\circ\pi)(X),...,(x^d\circ\pi)(X),(dx^1)_{\pi(x)}(X),...,(dx^d)_{\pi(X)}(X)\right)
\end{aligned}
$$
where $(x^i\circ\pi)(X)$ corresponds to projecting $X$ to base space $M$. Suppose this corresponds to a point $p$ on $M$ then $x^i(p)$ is the $i$ th component of $p\in u$ in chart $(u,x)$. And, $(dx^i)_{\pi(X)}(X) = (dx^i)_{\pi(X)}\left(X^j\frac{\partial}{\partial x^j}\right)_{\pi(X)} = X^j\delta^i_j = X^j$. So the map $\xi_x$ takes a vector $X$ from a tangent space $T_pM$ and maps it to a tuple where the first $d$ components correspond to components of $p$ in chart $x$ and the next $d$ components correspond to components of $X$ in chart $x$.

The inverse of this chart is as follows
$$
\begin{aligned}
\xi^{-1}_x:&\xi(Tu)\rightarrow Tu\\
&(\alpha^1,...,\alpha^d,\beta^1,...,\beta^d) := \beta^i\left(\frac{\partial}{\partial x^i}\right)_{(x^{-1}(\alpha^1,...,\alpha^d))}


\end{aligned}
$$

So this inverse if able to construct the full the vector in $Tu$. Is the defined chart smooth? 
Check

$$
\begin{aligned}
&(\xi_y \circ \xi_x^{-1})(\alpha^1,...,\alpha^d,\beta^1,...,\beta^d)\\
&= \xi_y(\beta^i(\frac{\partial}{\partial x^i})_{(x^{-1}(\alpha^1,...,\alpha^d))})\\
&= (..,(y^j\circ \pi)(\beta^i(\frac{\partial}{\partial x^i})_{(x^{-1}(\alpha^1,...,\alpha^d))}),..,(dy^j)_{(x^{-1}(\alpha^1,...,\alpha^d))}(\beta^i(\frac{\partial}{\partial x^i})_{(x^{-1}(\alpha^1,...,\alpha^d))}),..)\\
&= (..,(y^j\circ x^{-1})(\alpha^1,..,\alpha^d),.., \beta^i(\frac{\partial y^j}{\partial x^i})_{(x^{-1}(\alpha^1,..,\alpha^d))},..)
\end{aligned}
$$ 

We know that $(y^j\circ x^{-1})(\alpha^1,..,\alpha^d)$ is smooth by defintion of chart.  We can look at $\beta^i(\frac{\partial y^j}{\partial x^i})_{(x^{-1}(\alpha^1,..,\alpha^d))}$ we know in $\beta^{i}$ it is smooth. So we only look at $(\frac{\partial y^j}{\partial x^i})_{(x^{-1}(\alpha^1,..,\alpha^d))} =: \partial_i(y^j\circ x^{-1})(x(x^{-1}(\alpha^1,..,\alpha^d))) = \partial_i(y^j\circ x^{-1})(\alpha^1,..,\alpha^d)$ which is also smooth because the defined charts are smooth.