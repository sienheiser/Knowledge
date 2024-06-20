#math 
Chebyshev polynomials $T_n$ are an othogonal set on $[-1,1]$ for the measure $w = \frac{1}{\sqrt{1-x^2}}$. More precisely one has

$$
\int \frac{T_nT_m}{\sqrt{1-x^2}}dx = \frac{\pi}{2}(1+\delta_{0n})\delta_{nm}.
$$

All the other polynomials can be constructed using from $T_0 = 1$ and $T_1=x$ using recursive relation

$$
T_{n+1}(x) = 2xT_{n}(x)-T_{n-1}(x)
$$

### Properties

The Chebyshev polynomials have the following properties
- $T_n$ has the same partiy as $n$
- $T_n$ is of degree $n$
- $T_n(\pm 1) = (\pm 1)^N$
- $T_n$ has exactly $n$ zeros.

### Weights and collocation points for Gauss quadratures

- Chebysev-Gauss: $x_i = \cos(\frac{(2i+1)\pi}{2N+2}$ and $w_i = \frac{\pi}{N+1}$
- Chebysev-Gauss-Radau: $x_i = \cos(\frac{2\pi i}{2N+1})$. The weights are $w_0 = \frac{\pi}{2N+1}$ and $w_i = \frac{2\pi}{2N+1}$
- Chebysev-Gauss-Lobatto: $x_i = \cos(\frac{\pi i}{N})$. The weights are $w_0 = w_N = \frac{\pi}{N}$  and $w_i = \frac{\pi}{N}$

### Operators

Suppose we have function $f$ expanded in configuration space in terms of Legendre polynomials $f = \sum_{n=0}^N a_nT_n$. Suppose $H$ is an operator that does $Hf = \sum_{n=0}^N b_nT_n$. Relations between $b_n$ and $a_n$ can derived depending on what $H$ does
- If $H$ is a multiplication by $x$ then: $$b_n = \frac{1}{2}[(1+\delta_{0n-1})a_{n-1}+a_{n+1}]\quad (n\geq 1)$$
- If $H$ is a first order derivative: $$b_n = \frac{2}{1+\delta_{0n}}\sum_{p = n+1,p+n\text{ odd}}^N pa_p $$
-  If $H$ is a second order derivative: $$b_n = \frac{1}{1+\delta_{0n}}\sum_{p = n+2,p+n\text{ even}}^N p(p^2-n^2)a_p $$