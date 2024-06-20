---
aliases: [coefficient space, configuration space]
---
#math 

We have described how to project a function $u$ onto polynomials in [[Projecting Functions|projecting functions]]. Then we spoke about interpolation [[Interpolation|interpolation]] and how it differs from projecting function onto polynomials. It turns out a function $u$ can be described in terms of the collocation points used for interpolation or by the interpolants $\tilde{u}$ (which are essentially approximate coefficients). *If the values of the function $u$ are known at the collocation points $x_i$* then we are working in ***configuration space***. If the interpolants $\hat{u}$ are known then we are working in coefficient space. We can transform from one space to another by the following functions

$$
\tilde{u}_n = \frac{1}{\gamma_n}\sum_{j=0}^{N}u(x_j)p_n(x_j)w_j\quad (\text{configuration} \rightarrow \text{coefficient}) 
$$
$$
u(x_n) = \sum_{j = 0}^N\tilde{u}_jp(x_n)\quad (\text{coefficient} \rightarrow \text{configuration}) 
$$

where $\gamma_n$ is defined in [[Interpolation|interpolation]] and $p_j(x)$ are the basis polynomials. Depending on the operation one choice of space is prefered to another. 

For example suppose we want to compute the derivative of a function $u$ then this can be easily done if the coefficient space is known

$$
u^{'}(x) \approx [I_Nu]^{'} = \sum_{n=0}^N\tilde{u}_n p_n{'}(x)
$$
Note that the operations of differentiating and interpolanting do not communte, meaning the order of operations matter and will give different results. However with sufficient number of colocation points the they will converge to the same solution.