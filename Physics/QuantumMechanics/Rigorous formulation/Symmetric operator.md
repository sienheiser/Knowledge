***Definiton:*** A [[Physics/QuantumMechanics/Rigorous formulation/Dense|densely]] defined operator $A:\mathcal{D}_A\rightarrow H$ is called symmetric if 
$$
\forall \alpha,\beta\in \mathcal{D}_A\quad \langle A\alpha,\beta\rangle = \langle \alpha,A\beta\rangle.
$$



***Theorem:*** Let $A$ be a symmetric operator then the [[Self-adjoint and adjoint|adjoint]] of $A$ is an extenstion of $A$ i.e. $A\text{ symmetric}\implies A\subseteq A^*$.
*Proof:* Let $\psi\in\mathcal{D}_A$. Then define $\eta := A\psi$. Therefore if $\psi\in \mathcal{D}_{A^*}$ then $\forall\alpha\in\mathcal{D}_A \quad\langle \psi,A\alpha\rangle = \langle \eta,\alpha\rangle$. This can be shown by $\langle\eta,\alpha\rangle = \langle A\psi,\alpha\rangle = \langle\psi,A\alpha\rangle$. Therefore $\psi\in\mathcal{D}_{A^*}$.


***Observe:*** A self-adjoint operator implies a symmetric operator. But a symmetric operator does not imply a self-adjoint operator.



***Corollary:*** A self-adjoint operator $A$ cannot be further extended to another self-adjoint operator or symmetric operator.

*Proof:* Suppose $A$ and $B$ are self-adjoint operators and $B$ is an extension of $A$. Then $A\subseteq B \stackrel{1}{=} B^* \stackrel{2}{\subseteq}A^* \stackrel{3}{=} A$ where $\stackrel{1}{=},\stackrel{3}{=}$ are true because of the operators being self-adjoint and $\stackrel{2}{\subseteq}$ is true due to the second propsition in [[Propositions for adjoint operator]]. We see that $A\subseteq B$ and $B\subseteq A$. To show for extensition to symmetric operator simply replace $\stackrel{1}{=}$ with $\subseteq$.


***Proposition:*** If $A$ is a symmetric operator then $A^{**}\subseteq A^*$.
*Proof:* $A$ symmetric $\implies A\subseteq{A^*}\stackrel{1}{\implies}A^{**}\subseteq A^*$. Where $\stackrel{1}{\implies}$ is true because of proposition 2 in [[Propositions for adjoint operator]].  