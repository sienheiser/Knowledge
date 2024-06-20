*Theorem:* The point [[Spectrum|point spectrum]] of a [[Self-adjoint and adjoint|self-adjoint]] operator A
$$
\sigma_p(A) := \{z\in\sigma(A)|\overline{\text{ran}(A-z)\neq H}\}
$$
has as its elements precisely the eigenvalues of $A$

*Proof:* First we show that eigenvalues of a self adjoint operator $A$ are real.  Suppose $A\psi = \lambda\psi$ then
$$
\begin{aligned}
\lambda\langle \psi,\psi\rangle &= \langle \psi,\lambda\psi\rangle\\
&= \langle \psi,A\psi\rangle\\
&= \overline{\langle \psi,A\psi\rangle}\\
&= \bar{\lambda}\langle \overline{\psi,\psi}\rangle\\
&= \bar{\lambda}\langle \psi,\psi\rangle\\
&\implies \lambda = \bar{\lambda}.
\end{aligned}
$$

Now we show that $\lambda$ is an eigenvalue of $A$. We know
$$
\begin{aligned}
\{0\}&\stackrel{1}{\neq} \text{ker}(A-\lambda)\\
&= \text{ker}(A^*-\lambda)\\
&\stackrel{2}{=} \text{ker}(A-\bar{\lambda})^*\\
&\stackrel{3}{=} \text{ran}(A-\bar{\lambda})^\perp\\
&= \text{ran}(A-\lambda)^\perp
\end{aligned}
$$
This implies
$$
\begin{aligned}
&\overline{\text{ran}(A-\lambda)} = (\text{ran}(A-\lambda)^\perp)^\perp \neq \{0\}^\perp = H\\
&\implies \lambda\in\sigma_p(A)
\end{aligned}
$$

Conversely, suppose $\lambda$ is not an eigenvalue of $A$. Is $\bar{\lambda}$ not an eigenvalue either?
So

$$
\begin{aligned}
&\{0\} = \text{ker}(A-\bar{\lambda}) = \text{ker}(A^*-\bar{\lambda}) = \text{ker}((A-\bar{\lambda})^*) = \text{ran}(A-\lambda)^\perp\\
&\implies\overline{\text{ran}(A-\lambda)}=\text{ran}(A-\lambda)^{\perp\perp} = \{0\}^\perp = H\\
&\implies \lambda\notin\sigma_p(A).
\end{aligned}
$$