---
aliases: [interpolation]
---

We know from [[Projecting Functions|projecting functions]] that functions can be decomposed into polynomials that form an orthonormal basis. Suppose our function $u$ and we decompose it using  orthonormal set of polynomials $p_i$. Then we must get coefficients $\hat{u}_i$. These coefficients are expensive to compute. The solutions is to use [[Gauss Quadratures|Gauss quadratures]] to compute the coefficients that we will denote as $\tilde{u}_i$. The Gauss quadratures gives the approximated coefficients as 

$$
\tilde{u}_n = \frac{1}{\gamma_n}\sum_{j = 0}^N u(x_j)p_n(x_j)\quad\text{with}\quad \gamma_n = \sum_{j = 0}^(N)p_n^2(x_j)w_j.
$$

Important to note $\hat{u}_i \neq\tilde{u}_i$. However computing $\tilde{u}$ only required $N+1$ collocation points. The interpolation of function $u$ is given as

$$
I_N[u] = \sum_{n = 0}^N \tilde{u}_np_n(x).
$$

One can show that it is the only polynomial with degree $N$ that coincides with function $u$ at each collocation point

$$
[I_Nu](x_i) = u(x_i)\quad \forall i\leq N.
$$
The interpolant of $u$ is called the spectral approximant of $u$. 