*Theorem:* A symmetric operator $A$ is [[Self-adjoint and adjoint|self-adjoint]] if (but not only if)
$$
\exists z\in\mathbb{C}:\text{ran}(A+Z) = H = \text{ran}(A+\bar{z}).
$$

*Proof:* Since $A$ symmetric $\implies A\subseteq A^*$ by theorem in [[Symmetric operator|here]]. Remains to show $A^*\subseteq A$. 
Let $\psi\in\mathcal{D}_{A^*}$. Then consider $A^*\psi+\bar{z}\psi\in H$. Since $\text{ran}(A+\bar{z}) = H$
$$
\exists \rho\in\mathcal{D}_A:A^*\psi+\bar{z}\psi = (A+\bar{z})\rho.
$$
*I can see why this is true other than both belonging to $H$ therefore there is some overlap.* But then for any $\phi\in\mathcal{D}_A$

$$
\begin{aligned}
\langle \psi,(A+z)\phi\rangle &\stackrel{1}{=} \langle A^*\psi+\bar{z}\psi,\phi\rangle\\
&\stackrel{2}{=} \langle (A+\bar{z})\rho,\phi\rangle\\
&\stackrel{3}{=} \langle \rho,(A+z)\phi\rangle\\
&\stackrel{4}{\implies}\psi = \rho \in \mathcal{D}_A
\end{aligned}
$$
where $\stackrel{1}{=}$ is because $\psi\in\mathcal{D}_{A^*}$ therefore we need the adjoint,  $\stackrel{2}{=}$ is because of our assumption such a $\rho$ existing, $\stackrel{3}{=}$ is because $A$ is symmetric and $\rho,\phi\in\mathcal{D}_A$ and $\stackrel{4}{\implies}$ is because $\text{ran}(A+z)=H$ *not sure why we need this condition since we have shown that any element in* $\mathcal{D}_{A^*}$ also lies in $\mathcal{D}_A$.


*Remark:* If a symmetric operator does not satisfy the above condition, it does not mean that it is not a self-adjoint operator.