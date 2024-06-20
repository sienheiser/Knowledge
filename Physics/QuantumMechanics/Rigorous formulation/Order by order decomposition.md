We can plug the [[Formal power series ansatz|ansatz]] into the equation $H_\lambda e_{n\delta}(\lambda) = h_{n\delta}(\lambda)e_{n\delta}(\lambda)$. This gives

$$
\begin{aligned}
LHS &= (H_0+\lambda W)(e_{n\delta}+\lambda\epsilon^{(1)}_{n\delta}+\lambda^2\epsilon^{(2)}_{n\delta}+\mathcal{O}(\lambda^3))\\
&= H_0e_{n\delta}+\lambda(W e_{n\delta}+H_0\epsilon_{n\delta}^{(1)})+\lambda^2(W\epsilon_{n\delta}^{(1)}+H_0\epsilon_{n\delta}^{(2)})
\end{aligned}
$$
The other side of the equation becomes

$$
\begin{aligned}
RHS &= (h_n+\lambda\theta^{(1)}_{n\delta}+\lambda^2\theta^{(2)}_{n\delta}+\mathcal{O}(\lambda^3))(e_{n\delta}+\lambda\epsilon^{(1)}_{n\delta}+\lambda^2\epsilon^{(2)}_{n\delta}+\mathcal{O}(\lambda^3))\\
&=h_ne_{n\delta}+\lambda(h_n\epsilon^{(1)}_{n\delta}+\theta^{(1)}e_{n\delta})+\lambda^2(h_n\epsilon^{(2)}_{n\delta}+\theta^{(1)}_{n\delta}\epsilon^{(1)}_{n\delta}+\theta^{(2)}_{n\delta}e_{n\delta})\\
\end{aligned}
$$
Comparing the $LHS$ and $RHS$ we see

$$
\begin{aligned}
&\lambda^{0}:(H_0-h_n)e_{n\delta} = 0\\
&\lambda^{1}:(H_0-h_n)\epsilon^{(1)}_{n\delta} = -(W-\theta_{n\delta}^{(1)})e_{n\delta}\\
&\lambda^2:(H_0-h_n)\epsilon_{n\delta}^{(2)} = -(W-\theta^{(1)}_{n\delta})\epsilon_{n\delta}^{(1)}+\theta_{n\delta}^{(2)}e_{n\delta}
\end{aligned}
$$




