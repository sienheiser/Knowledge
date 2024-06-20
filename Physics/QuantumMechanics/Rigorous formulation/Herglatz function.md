*Theorem:*
$$
\begin{aligned}
\langle\psi,R_A(\cdot)\psi\rangle:&\mathbb{C}^+\rightarrow\mathbb{C}^+\\
&z\mapsto \frac{1}{\lambda-z}

\end{aligned}
$$



where $\mathbb{C}^+:=\{z\mathbb{C}|\Im(z)\geq 0\}$. This property is also known as a Herglatz function. 

Being a Herglatz function implies that the measure $\mu_\psi\geq0$.

*Proof:*

$$
\begin{aligned}
\Im(\langle\psi,R_A(z)\psi\rangle)&=\Im\int\frac{1}{\lambda-z}\mu_\psi(d\lambda)\\
&= \int_\mathcal{R}\frac{\Im(z)}{|\lambda-z|^2}\mu_\psi(d\lambda)\\
&= \Im(z)\int_\mathcal{R}\frac{1}{|\lambda-z|^2}\mu_\psi(d\lambda)
\end{aligned}
$$
which clearly takes $z\in\mathbb{C}^+$ and maps it to another $z\in\mathbb{C}^+$.