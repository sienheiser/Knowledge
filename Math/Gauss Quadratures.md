---
aliases: [Gauss quadratures]
---
#math 
#NotHappyWithExplanation 

We know we can project functions onto polynomials from [[Projecting Functions|projecting functions]]. However, each time we compute a coefficent for the projection we have to compute the [[scalar product]] which is an integral. So if we compute a the projection of the function $u$ at many points then it becomes computationally expansive (***what do you mean by many points?***). The solution is to use Gauss quadratures. The theorem can be stated as follows. *There exists* $N+1$ *positive reals* $w_n$ and $N+1$ reals $x_n$ *in* $\Lambda$ *such that*
$$
\forall f \text{ belonging to } \mathbb{P}_{2N+\delta},\int f(x)w(x)dx = \sum_{i = 0}^Nf(x_i)w_i.
$$
The $w_i$ are called the weigths and the $x_i$ are called the [[collocation points ]] (basically nodes that are chosen to approximante the function). There are three usual choices for $\delta$ 

- Gauss: $\delta = 1$
- Gauss-Raudau: $\delta = 0$ and $x_0 = x_{min}$
-  Gauss-Lobatto: $\delta = -1$ and $x_0 = x_{min}$ and $x_N = x_{max}$


where $x_{min}$ is the minimum $x$ in an interval and $x_{max}$ is the maximum x value in the interval.