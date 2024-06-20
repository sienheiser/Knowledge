---
aliases: [reconstructing PVM]
---

Let $A\stackrel{*}{=}\int \lambda P(d\lambda)$ (where the $*$ will be used later) for some [[Projection valued measure (PVM)|PVM]] P. Then the [[Resolvent maps|resolvent map]] $R_A(z)$ for $z\in\rho(A)\subseteq\mathbb{C}$ can be written as
$$
R_A(z) = (A-z)^{-1}=r_z(A)\stackrel{*}{=}\int r_zdP :=\int\frac{1}{\lambda-z}P(d\lambda)
$$
for any $\psi\in H$.

This implies 
$$
\begin{aligned}
\langle\psi,R_A(Z)\psi\rangle &= \langle\psi,(\int r_z dP)\psi\rangle\\
&\stackrel{1}{=}\int_{\mathbb{R}}r_z d\mu_\psi\\
&=\int_{\mathbb{R}}\frac{1}{\lambda-z}\mu_\psi(d\lambda).
\end{aligned}
$$

Where $\stackrel{1}{=}$ is true because of step 2 [[Integration w.r.t PVM over simple functions|here]]. Now $\langle\psi,R_A(Z)\psi\rangle$ is also known as a [[Herglatz function]] which ensures that $\mu_\psi\geq 0$. 