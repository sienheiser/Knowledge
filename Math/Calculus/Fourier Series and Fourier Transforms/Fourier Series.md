If a function $f(x)$ satifies the [[Dirichlet Conditions|Dirichlet conditions]] then it be written as

$$
f(x) = \frac{a_0}{2}+\sum_{n=1}^{\infty}a_n \cos(\frac{2\pi n x}{L})+b_n\sin(\frac{2\pi n x}{L})
$$
where the RHS is called the Fourier series of the function.


If the function is even $f(-x) = f(x)$ then all $b_n = 0$, if the function is odd $f(x) = -f(x)$ then all $a_n = 0$. To find the coefficients we rewrite the series as 

$$
f(x) = \sum_{n=-\infty}^{\infty} C_n \exp(\frac{2\pi i n x}{L}).
$$
Then integrate both sides over an entire period giving

$$
\int_{x_0}^{x_0+L}f(x)\exp(\frac{-2\pi i k x}{L})dx = \sum_{n =-\infty}^{\infty}\int_{x_0}^{x_0+L}C_n\exp(\frac{2\pi(n-k)x}{L})dx.
$$
The right hand side integral is equal to 
$$
\int_{x_0}^{x_0+L}C_n\exp(\frac{2\pi(n-k)x}{L})dx = L\quad \text{for}\quad n = k
$$
otherwide it is equal to zero. Thus we get 
$$
C_k = \frac{1}{L}\int_{x_0}^{x_0+L}f(x)\exp(\frac{-2\pi i k x}{L})dx
$$