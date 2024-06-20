*Theorem 1:* A symmetric operator $A$ is [[Essentially self adjoint operators|essentially self-adjoint]] iff
$$
\exists z\in\mathbb{C}\backslash\mathbb{R}:\overline{\text{ran}(A+z)}=H=\overline{\text{ran}(A+\bar{z})}
$$
*Proof:* Literature

*Theorem 2:* A symmetric operator $A$ is essentially self-adjoint iff
$$
\exists z\in\mathbb{C}\backslash\mathbb{R}:\text{ker}(A^*+\bar{z})=\{0\}=\text{ker}(A^*+z)
$$
*Proof:*  $\overline{\text{ran}(A+z)}\stackrel{1}{=} \text{ran}(A+z)^{\perp\perp}\stackrel{2}{=} (\text{ker}(A+z)^*)^\perp \stackrel{3}{=} \text{ker}(A^*+\bar{z})^\perp$. Not sure why $\stackrel{1}{=}$ is true, $\stackrel{2}{=}$ is true because of proposition 1 in [[Propositions for adjoint operator]] and $\stackrel{3}{=}$ is true because of $\bar{z}$ is just a complex number. Similarly we can show that $\overline{\text{ran}(A+\bar{z})} =\text{ker}(A^*+z)^\perp$. Then from the above theorem 1 we have essentially self adjoint.