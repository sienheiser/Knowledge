### Ajoint
To calculate the [[Self-adjoint and adjoint|adjoint]] of the momentum operator in a 1D ring we may use results from [[Adjoint of 1D momentum operator (infinite well)]]. The condition for a function to belong to a domain of momentum operator for infinite well is $\psi(0)=\psi(2\pi)=0$. While to belong to the domain of momentum operator for 1D ring $\psi(0)=\psi(2\pi)$. Clearly the condition for inifnite well is stronger than for 1D therefore $\mathcal{D}_{p_{\text{interval}}}\subseteq\mathcal{D}{p}$ where ${D}_{p_{\text{interval}}}$ is domain for infinite well and $\mathcal{D}{p}$ is domain for 1D ring. This means $p_{\text{interval}}\subseteq p$ where $p$ is the momentum operator. By [[Propositions for adjoint operator| proposition 2]] $p^{*}\subseteq p^{*}_{\text{interval}}$.

Now using definiton of [[Self-adjoint and adjoint|adjoint]] we have $\psi\in\mathcal{D}_{p^{*}}\implies\forall \phi\in\mathcal{D}_p:\langle\psi,p\phi\rangle=\langle p^{*}\psi,\phi\rangle = \langle p^{*}_{\text{interval}}\psi,\phi\rangle$. Then
$$
\begin{aligned}
\int_{0}^{2\pi}\bar{\psi}(-i)\phi'dx &= \int_{0}^{2\pi} \overline{-i\psi'}\phi dx\\
\iff [\bar{\psi}\phi]_{0}^{2\pi} &= 0
\end{aligned}
$$
Since $\phi\in\mathcal{D}_p$ then $0=[\bar{\psi}\phi]_{0}^{2\pi}=\phi(0)(\psi(2\pi)-\psi(0))$ is only true if $\psi(2\pi)=\psi(0)$. Therefore $\mathcal{D}_{p^*}:=\{\psi\in H^1([0,2\pi])|\psi(2\pi)=\psi(0)\}$. Therefore $p\subsetneq p^{*}$ since $p$ only acts on once continously differentiable funcitons.

### Essentially self adjoint
Since $p$ is [[Symmetric operator|symmetric]] then $p\subseteq p^{**}\subseteq p^{*}$. Using $\psi\in\mathcal{D}_{p^{**}}:\forall \phi\in\mathcal{D}_{p^{*}}:\langle\psi,p^{*}\phi\rangle=\langle p^{**}\psi,\phi\rangle=\langle p^{*}\psi,\phi\rangle$ we again get 
$$
[\psi\phi]_{0}^{2\pi} = 0 = \phi(0)(\psi(2\pi)-\psi(0))
$$
which is only true if $\psi(2\pi)=\psi(0)$ therefore we see $\mathcal{D}_{p^{**}}=H^1_{\text{cyclic}}=\mathcal{D}_{p^{*}}$ which means $p^{**}=p^{*}\iff p^{***}=p^{**}$ which is essentially self-adjoint.
