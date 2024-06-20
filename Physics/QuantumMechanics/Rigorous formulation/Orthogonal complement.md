*Definition:* Let $M$ be a (not necessarily closed) [[Linear subspace|linear subspace]] of $\mathit{H}$. Then the set 
$$
M^\perp := \{\psi\in\mathit{H} | \forall \mu\in M:\langle\mu,\psi\rangle = 0\}
$$
is the orthogonal complement. Basically take any element in $\mathit{H}$ and if its inner products for all  $\mu\in M$ is zero it belongs to $M^\perp$.

*Property:* $M^\perp$ is a closed linear subspace of $\mathit{H}$.
*Proof:* We show that it is a linear subspace. Suppose $\psi_1,\psi_2\in M^\perp$. Then since the inner product is linear in the second argument $\psi_1+\psi_2\in M\perp$ and $\lambda\cdot\psi_1\in M^\perp$ for any $\lambda\in \mathbb{C}$.

We show that it is closed. First rewrite $M^\perp$ as
$$
M^\perp = \bigcap_{\mu\in M} \text{preim}_{\omega_\mu}(\{0\})
$$
where
$$
\begin{aligned}
\omega_\mu:&\mathit{H}\rightarrow \mathbb{C}\\

&\psi\mapsto \langle\mu,\psi\rangle.
\end{aligned}
$$

Clearly the $\text{preim}_{\omega_\mu}(\{0\})$ for a $\mu$ is all the vectors $\psi_i\in\mathit{H}$ where $\langle\mu,\psi\rangle = 0$. If we show that for arbitrary $\mu$ that $\text{preim}_{\omega_\mu}(\{0\})$ is closed then we know from topology that arbitrary intersection of closed sets is closed. 

Consider
$$
\begin{aligned}
\mathit{H}/ \text{preim}_{\omega_\mu}(\{0\}) &= \{\psi\in\mathit{H}|\langle\mu,\psi\rangle\neq 0\}\\

&= \{\psi\in\mathit{H}|\langle\mu,\psi\rangle\in \mathbb{C}/\{0\} \}\\

&= \text{preim}_{\omega_\mu}(\mathbb{C}/\{0\})
\end{aligned}
$$

We know that $\mathbb{C}/\{0\}$ is open since $\{0\}$ is closed in the standard topology on $\mathbb{C}$. Since the inner product is continous we know the $\text{preim}_{\omega_\mu}(\mathbb{C}/\{0\})$ is also open in $\mathit{H}$ by definiton of continuity in topology. Therefore $\mathit{H}/ \text{preim}_{\omega_\mu}(\{0\})$ is open meaning $\text{preim}_{\omega_\mu}(\{0\})$ is closed for arbitrary $\mu$. Which finally means that $M^{\perp}$ is also closed.
