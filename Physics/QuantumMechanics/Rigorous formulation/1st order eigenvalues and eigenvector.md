Using $\lambda^1$ from [[Order by order decomposition]] we get 

$$
\langle e_{n\alpha},(H_0-h_n)\epsilon_{n\delta}^{(1)} \rangle = \langle e_{n\alpha},(W-\theta^{(1)}_{n\delta})e_{n\delta} \rangle.
$$
Looking at $LHS = \langle e_{n\alpha},(H_0-h_n)\epsilon_{n\delta}^{(1)} \rangle\stackrel{H_0=H_0^*}{=}\langle (H_0-h_n)e_{n\alpha},\epsilon_{n\delta}^{(1)} \rangle = \langle 0,\epsilon_{n\delta}^{(1)} \rangle = 0$. Then $RHS$ can be rewritten as $\langle e_{n\alpha},We_{n\delta}\rangle=\langle e_{n\alpha},\theta^{(1)}_{n\delta}e_{n\delta}\rangle=\theta_{n\delta}^{(1)}\delta_{\delta\alpha} = \theta^{(1)}_{n\alpha}$ Therefore
$$
\theta^{(1)}_{n\alpha}=\langle e_{n\alpha},We_{n\delta}\rangle
$$

So we have found first order correction to pertubation of eigenvalue. Now we find first order correction for eigenvector. We have $RHS$ from $\lambda^1$ as 
$$
\begin{aligned}
RHS &= -(W-\theta_{n\delta}^{(1)})e_{n\delta}=-(P_E+P_{E^\perp})(W-\theta_{n\delta}^{(1)})e_{n\delta}\\
&= -\sum_{\beta = 1}^{d(n)}\langle e_{n\beta},(W-\theta_{n\delta}^{(1)})e_{n\delta}\rangle e_{n\beta}-P_{E^\perp}(W-\theta_{n\delta}^{(1)})e_{n\delta}\\
&= -P_{E^\perp}(W-\theta_{n\delta}^{(1)})e_{n\delta}\\
\end{aligned}
$$
where last equality is true because of $\theta^{(1)}_{n\delta}$ and $E:= \text{Eig}_{H_0}(h_n)$. We see that $RHS\in\text{Eig}_{H_0}(h_n)^\perp$. Therefore, restricting $\lambda^1$  to $P_{E^\perp}$ allows us to invert $(H_0-h_n)$ giving
$$
\begin{aligned}
\epsilon_{n\delta}^{(1)} &= -P_{E^\perp}(H_0-h_n)^{-1}P_{E^\perp}((W-\theta_{n\delta}^{(1)})e_{n\delta})+\sum_{\beta=1}^{d(j)}c_{\delta\beta}e_{n\beta}\\
&= -P_{E^\perp}(H_0-h_n)^{-1}P_{E^\perp}(We_{n\delta})+\sum_{\beta=1}^{d(j)}c_{\delta\beta}e_{n\beta}
\end{aligned}
$$
where the last equality is true  $\theta_{n\delta}^{(1)}P_{E^\perp}e_{n\delta} = 0$ and the sum term is an extra contribution due to inverting the operator.