Suppose we have curve $x^{\mu}(\lambda)$ in flat space and a tensor $T^{\alpha\beta}$. Then parallel transporting this tensor means 

$$
\frac{d}{d\lambda}T^{\alpha\beta} = \frac{d x^{\mu}}{d\lambda} \frac{\partial T^{\alpha\beta}}{\partial x^{\mu}} = 0.
$$

To generalize this to curve space we replace the partial derivative with a [[Covariant Derivative|covariant derivative]]  giving
$$
\frac{D}{d\lambda}T^{\alpha\beta} = \frac{dx^{\mu}}{d\lambda}\nabla_{\mu}T^{\alpha\beta} = 0.
$$

For a vector in curved space the parallel transport equation takes form

$$
\begin{aligned}
&\frac{dx^{\nu}}{d\lambda}\left(\frac{\partial V^{\mu}}{\partial x^{\nu}}  + \Gamma_{\nu\sigma}^{\mu}V^{\sigma} \right)\\
&= \frac{dx^{\nu}}{d\lambda}\frac{\partial V^{\mu}}{\partial x^{\nu}} + \frac{dx^{\nu}}{d\lambda} \Gamma_{\nu\sigma}^{\mu}V^{\sigma}\\
&= \frac{d V^{\mu}}{d\lambda} + \Gamma_{\nu\sigma}^{\mu}\frac{dx^{\nu}}{d\lambda}V^{\sigma}\\
&= 0
\end{aligned}
$$