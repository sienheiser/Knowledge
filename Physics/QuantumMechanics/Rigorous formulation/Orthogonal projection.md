*Definiton:* Suppose we have Hilbert space $H$ and a closed [[Linear subspace]] $M$. The map
$$
\begin{aligned}
P_M:&H\rightarrow M\\
&= \psi\mapsto \psi_\|
\end{aligned}
$$
where $\psi_\|=\sum \langle e_i,\psi\rangle e_i$ is called the orthogonal projector to the sub-Hilbert space $M$.


Properties:
 1. $P_M\circ P_M = P_M$
 2. $\psi,psi\in H: \langle P_M\psi,\phi=\langle\psi,P_M\phi\rangle$
 3. $P_{M^\perp}:H\rightarrow M^\perp$ takes $\psi\mapsto \psi_\perp$.
 4. $P_M\in\mathcal{L}(H,M)$. So it is a bounded map


*Proof:*