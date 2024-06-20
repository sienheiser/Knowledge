#math

The Legendre polynomials, denoted by $P_n$, constitute a family of orthgonal polynomials on \[-1,1] with a [[Math/MeasureTheory/measure]] of $w = 1$. The [[scalar product]] of two Legendre polynomials is given as

$$
\int_{-1}^1P_nP_mdx = \frac{2}{2n+1}\delta_{nm}.
$$

Given that $P_0 = 1$ and $P_1 = x$, all other Legendre polynomials can be constructed using recursive relation 

$$
(n+1)P_{n+1}(x)= (2n+1)xP_n(x)-nP_{n-1}(x).
$$

### Properties
The Legendre polynomials have the following properties 

- $P_n$ has the same parity of $n$
- $P_n$ is a polynomial of degree $n$
- $P_n(\pm1) = (\pm 1)^n$
- $P_n$ has exactly $n$ roots in interval $[-1,1]$


### Weights and collocation points for Gauss quadratures

The weights and collocation points for Legendre polynomials used in [[Gauss Quadratures|Gauss quadratures]] are (there are three different methods) 
- Legendre-Gauss: $x_i$ are the nodes (***roots?***) of $P_{N+1}$ and $w_i = \frac{2}{(1-x_i^2)[P^{'}_{N+1}(x_i)]^2}$
- Legendre-Gauss-Radau: $x_0 = -1$ and $x_i$ are the nodes (***roots?***) of $P_N$ and $w_i = \frac{1}{(N+1)^2}$
- Legendre-Gauss-Lobatto: $x_0 = -1$, $x_N = 1$ and $x_i$ are nodes (***roots?***) of $P_N^{'}$. The weights are $w_i = \frac{2}{N(N+1)}\frac{1}{P_N(x_i)^2}$


Position of collocation points are not analytic and need to be computed numerically. 

### Operators

Suppose we have function $f$ expanded in configuration space in terms of Legendre polynomials $f = \sum_{n=0}^N a_nP_n$. Suppose $H$ is an operator that does $Hf = \sum_{n=0}^N b_nP_n$. Relations between $b_n$ and $a_n$ can derived depending on what $H$ does

- If $H$ is a multiplication by $x$ then: $$b_n = \frac{n}{2n-1}a_{n-1}+\frac{n+1}{2n+3}a_{n+1}\quad (n\geq 1)$$
- If $H$ is a first order derivative: $$b_n = (2n+1)\sum_{p = n+1,p+n\text{ odd}}^N a_p $$
-  If $H$ is a second order derivative: $$b_n = (n+\frac{1}{2})\sum_{p = n+2,p+n\text{ even}}^N a_p $$

These kinds of relations allows us to represent $H$ as a matrix acting on a vector $a$ and giving another vector $b$.



