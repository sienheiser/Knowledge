*Definiton:* The spectrun $\sigma(A):=\mathbb{C}\backslash \rho(A)$ where $\rho(A)$ is the [[Resolvent maps|resolvent set]].



*Corollary:* $\lambda\in\mathbb{C}$ is an eigenvalue of an operator $A:\mathcal{D}_A\rightarrow H$ i.e. $\exists \psi\in\mathcal{D}_A\backslash\{0\}:A\psi=\lambda\psi$, then it follows $\lambda\in\sigma(A)$.

*proof:* $0\neq\psi\in\text{ker}(A-\lambda)$, ie. $\text{ker}(A-\lambda)\neq 0\implies A-\lambda$ is not [[Injective|injective]] $\implies \lambda\notin\rho(A)\implies \lambda\in\sigma(A)$.


### decomposition of spectrum

In general the spectrum $\sigma(A)$ can be decomposed into the following mutually exclusive sets
$$
\begin{aligned}
\sigma(A)_{\text{pure point}} := &\{z\in\mathbb{C}|\text{ran}(A-z) = \overline{\text{ran}(A-z)}\neq H\}\\
\sigma(A)_{\text{point in continuum}}:=&\{z\in\mathbb{C}|\text{ran}(A-z)\neq \overline{\text{ran}(A-z)}\neq H\}  \\
\sigma(A)_{\text{continuum}}:= &\{z\in\mathbb{C}|\text{ran}(A-z)\neq \overline{\text{ran}(A-z)}= H\}  \\
\end{aligned}
$$

The first and second set combined are called the ***point spectrum***. The second and third set are called ***continuum spectrum***.