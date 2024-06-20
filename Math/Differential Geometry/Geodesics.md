*Defintion:* A curve $\gamma:(0,1)\rightarrow M$ is called a geodesic on a Riemannian mfd $(M,\mathcal{O},\mathcal{A},g)$ if it is a stationary curve w.r.t the [[Length of curve|length functional]] $L$.

We may interpret the length functional as a Lagrangian which means $\sqrt{g(\mathcal{v}_\gamma,\mathcal{v}_\gamma)}$ satisfies the [[Euler-Lagrange Equations|Euler-Lagrange Equations]]. Therefore
$$
\begin{aligned}
 \frac{\partial\mathcal{L}}{\partial \dot{\gamma}^m} &= \frac{\partial}{\partial \dot{\gamma}^m}\sqrt{g_{ij}(\gamma{\lambda})\dot{\gamma}^i\dot{\gamma}^j}\\
 &= \frac{g_{mj}\dot{\gamma}^j}{\sqrt{g(\gamma(\lambda))_{ij}\dot{\gamma}^i\dot{\gamma}^j}}
\end{aligned}
$$
Then taking the derivative w.r.t to $\lambda$ gives
$$
\begin{aligned}

\frac{d}{d\lambda}\frac{\partial\mathcal{L}}{\partial \dot{\gamma}^m} = \frac{d}{d\lambda}\left(\frac{1}{\sqrt{g(\gamma(\lambda))_{ij}\dot{\gamma}^i\dot{\gamma}^j}} \right)g_{mj}\dot{\gamma}^j+\frac{(\partial_s g_{mj}\dot{\gamma}^s\dot{\gamma}^j+g_{mj}\ddot{\gamma}^j)}{\sqrt{g(\gamma(\lambda))_{ij}\dot{\gamma}^i\dot{\gamma}^j}}

\end{aligned}
$$
Then we can choose a parametrization such that $\sqrt{g(\gamma(\lambda))_{ij}\dot{\gamma}^i\dot{\gamma}^j} = 1$. Then the first term in the above equation goes to zero.

We compute the next term in the Euler-Lagrange equation
$$
\frac{\partial\mathcal{L}}{\partial \gamma^m} = \frac{\partial_s g_{ij}\dot{\gamma}^i\dot{\gamma}^j}{2\sqrt{g(\gamma(\lambda))_{ij}\dot{\gamma}^i\dot{\gamma}^j}}
$$
The denominator is equal to one since we have chosen such a parameterization. Colleting all the terms on one side yields

$$
g_{mj}\ddot{\gamma}^j+\partial_s g_{mj}\dot{\gamma}^s\dot{\gamma}^j-\frac{\partial_s g_{ij}\dot{\gamma}^i\dot{\gamma}^j}{2} = 0
$$

which can be rewritten as
$$
g_{mj}\ddot{\gamma}^j+\frac{1}{2}(\partial_i g_{mj}+\partial_j g_{mi}-\partial_s g_{ij})\dot{\gamma}^i\dot{\gamma}^j = 0
$$

Multiply on both sides by $g^{mq}$ giving
$$
\ddot{\gamma}^q+\frac{g^{mq}}{2}(\partial_i g_{mj}+\partial_j g_{mi}-\partial_s g_{ij})\dot{\gamma}^i\dot{\gamma}^j = 0
$$
This is an [[Autoparallel equation|autoparallel equation]] is $\Gamma^q_{ij} = \frac{g^{mq}}{2}(\partial_i g_{mj}+\partial_j g_{mi}-\partial_s g_{ij})$. Therefore, given a metric $g$ it is possible to specify a connection using the metric. This connection is called the Levi-Civita connection.


