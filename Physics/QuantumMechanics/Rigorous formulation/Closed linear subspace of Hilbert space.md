Not any [[Linear subspace]] of a seperable Hilbert space is  a seperable sub-Hilbert space, for it may fail to be complete.

*Lemma:* A closed subset $M\subseteq \mathit{H}$ of  a complete space is again complete.

*Proof:* Strategy: We take any [[Cauchy sequence]] $\{\psi_n\}$ in $M\subseteq\mathit{H}$; show that its limit exists and that the limit is an element of $M$.

Since $\{\psi_n\}\subseteq M\subseteq\mathit{H}$ then is has a limit since the Hilbert space is complete.

Suppose that 
$$
\lim_{n\rightarrow\infty}\psi_n \notin M.
$$
Since $M$ is topologically closed we know that $\mathit{H}/M$ is open. Furthermore there should be some set $U\subseteq\mathit{H}/M$ where the  limit of the sequence exists. This also means after a certain $m$ of the Cauchy sequence $\psi_m$ all $\psi_m\in \mathit{H}/M$. However this is a contradiction since all of our sequence $\{\psi_n\}$ lies in set $M$ but $\mathit{H}/M$ contains no element of $M$ therefore the assumption is wrong and
$$
\lim_{n\rightarrow\infty}\psi_n \in M.
$$


*Corollary:* A clodes linear subspace $M\subseteq \mathit{H}$ is a subHilbert space. If $\mathit{H}$ is seperable so it $M$.
