We defined the [[Self-adjoint and adjoint|adjoint]] operator. We have two important propositions. Suppose we have a Hilbert space $H$.

*Proposition 1:* $\text{ker}(A^*) = \text{ran}(A)^\perp$ where $\text{ran}(A):= A(\mathcal{D}_A)$ and $\text{ran}(A)^\perp$ is the [[Orthogonal complement|orthogonal complement]].
Proof: 
$$
\begin{aligned}
\text{ker}(A^*)&:= \{\psi\in H|A^*\psi = 0\}\\
\text{ran}(A)^\perp&:= \{\psi\in H|\forall \phi\in\mathcal{D}_A\langle \psi,\phi\rangle = 0\} 
\end{aligned}
$$

Suppose $\psi\in\text{ker}(A^*)$. This is equivalent to $A^*\psi = 0$. By definiton this means $\forall \alpha\in H\quad 0=\langle 0,\alpha\rangle = \langle \psi,A\alpha\rangle$ which means $\psi\in\text{ran}(A)^\perp$.


*Proposition 2:* Suppose we have two operators $A$,$B$ where $B$ is an extenstion of $A$ (denoted as $A\subseteq B$) which means $\mathcal{D}_A\subseteq\mathcal{D}_B$ and $A\alpha = B\alpha\quad\forall\alpha\in\mathcal{D}_A$.  Then $A\subseteq B\implies B^*\subseteq A^*$.
Proof:
$$
\begin{aligned}
\mathcal{D}_{A^*} &= \{\psi\in\mathit{H}|\forall \alpha\in \mathcal{D}_A\quad \exists \eta\in\mathit{H}:\langle\psi,A\alpha\rangle = \langle\eta,\alpha\rangle\}\\

\mathcal{D}_{B^*} &= \{\psi\in\mathit{H}|\forall \beta\in \mathcal{D}_B\quad \exists \eta\in\mathit{H}:\langle\psi,A\beta\rangle = \langle\eta,\beta\rangle\}
\end{aligned}
$$
Since $\mathcal{D}_{A}\subseteq\mathcal{D}_{B}$ the condition on $\mathcal{D}_{B^*}$ is stronger, therefore less $\psi\in H$ satisfy this condition. This means $\mathcal{D}_{B^*}\subseteq \mathcal{D}_{A^*}$.