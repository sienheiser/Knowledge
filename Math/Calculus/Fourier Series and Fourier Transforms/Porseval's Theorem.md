#Calculus 

It is some sort of conservation law. It relates the sum of the moduli squared $C_n$ to the average value of $|f(x)|^2$ over one period.

Consider two functions $f(x)$ and $g(x)$ where both of them have their own [[Fourier Series|Fourier series]]. Then if we take integral
$$
\frac{1}{L}\int_{x_0}^{x_0+L}f(x)g^*(x)dx
$$
 and expand $f(x)$ in terms of its Fourier series we get
 
 $$
 \frac{1}{L}\sum_{n=-\infty}^{\infty}C_n\int_{x_0}^{x_0+L}g^*(x)\exp(\frac{2\pi i nx}{L})dx = \frac{1}{L}\sum_{n=-\infty}^{\infty}C_n\left(\int_{x_0}^{x_0+L}g(x)\exp(-\frac{2\pi i nx}{L})dx\right)^*
 $$
 where the term in the brackets is just the coeffiecents of the Fourier series for $g(x)$. This gives the final integral as
 
$$
\frac{1}{L}\int_{x_0}^{x_0+L}f(x)g^*(x)dx = \sum_{n=-\infty}^{\infty}C_n\gamma_n^*
$$
where $\gamma_n$ are the Fourier coefficents of $g(x)$. If $g(x) = f(x)$ then we get the following relation
$$
\frac{1}{L}\int_{x_0}^{x_0+L}|f(x)|^2dx = \sum_{n=-\infty}^{\infty}|C_n|^2
$$
which is reminiscent of the quantum mechanics normalization of a wave function.