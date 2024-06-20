#DifferentialGeometry 

Suppose we have a smooth manifold where two charts $(U,x)$ and $(V,y)$ intersect. We want to find the relation between the connection coefficients of the $y$ and $x$ chart. We can do this using [[Transformation laws|transformation laws]]. Then
$$
\begin{aligned}
\Gamma_{(y)jk}^i &:= dy^i(\nabla_{\frac{\partial}{\partial y^k}}\frac{\partial}{\partial y^j})\\

&=\frac{\partial y^i}{\partial x^a}dx^a\left(\nabla_{\frac{\partial x^b}{\partial y^k}\frac{\partial}{\partial x^b}}\frac{\partial x^c}{\partial y^j}\frac{\partial}{\partial x^c}\right)\\

&= \frac{\partial y^i}{\partial x^a}\frac{\partial x^b}{\partial y^k}dx^a\left(\nabla_{\frac{\partial}{\partial x^b}}\frac{\partial x^c}{\partial y^j}\frac{\partial}{\partial x^c}\right)\\

&=\frac{\partial y^i}{\partial x^a}\frac{\partial x^b}{\partial y^k}dx^a\left(\nabla_{\frac{\partial}{\partial x^b}}(\frac{\partial x^c}{\partial y^j})\frac{\partial}{\partial x^c} + \frac{\partial x^c}{\partial y^j}\nabla_{\frac{\partial}{\partial x^b}} (\frac{\partial}{\partial x^c}) \right)\\

&= \frac{\partial y^i}{\partial x^a}\frac{\partial x^b}{\partial y^k}dx^a  \left(\frac{\partial}{\partial x^b}(\frac{\partial x^c}{\partial y^j})\frac{\partial}{\partial x^c} + \frac{\partial x^c}{\partial y^j}\Gamma_{(x)cb}^e\frac{\partial}{\partial x^e} \right)\\

&= \frac{\partial y^i}{\partial x^a}\frac{\partial x^b}{\partial y^k}\left(\frac{\partial}{\partial x^b} (\frac{\partial x^c}{\partial y^j})dx^a(\frac{\partial}{\partial x^c})+ \frac{\partial x^c}{\partial y^j}\Gamma_{(x)cb}^e dx^a(\frac{\partial}{\partial x^e})   \right)\\

&= \frac{\partial y^i}{\partial x^a}\frac{\partial x^b}{\partial y^k}\left(\frac{\partial}{\partial x^b} (\frac{\partial x^a}{\partial y^j})+ \frac{\partial x^c}{\partial y^j}\Gamma_{(x)cb}^a   \right)\\

&= \frac{\partial y^i}{\partial x^a}\frac{\partial x^b}{\partial y^k}\frac{\partial}{\partial x^b} (\frac{\partial x^a}{\partial y^j}) + \frac{\partial y^i}{\partial x^a}\frac{\partial x^b}{\partial y^k}\frac{\partial x^c}{\partial y^j}\Gamma_{(x)cb}^a\\

&= \frac{\partial y^i}{\partial x^a}\frac{\partial^2 x^a}{\partial y^k\partial y^j} + \frac{\partial y^i}{\partial x^a}\frac{\partial x^b}{\partial y^k}\frac{\partial x^c}{\partial y^j}\Gamma_{(x)cb}^a\\
\end{aligned}
$$

*Remark*: In the last equality we introduce a double derivative, we could not do this before because we had derivates from two different charts.