---
aliases: [PVM]
---
#ToBeProven
*Definiton:* Given a [[Borel sigma algebra|Borel set]] $\sigma(\mathcal{O})$ a map $P:\sigma(\mathcal{O})\rightarrow \mathcal{L}(H)$ is called a PVM if
1. $\forall\Omega\in\sigma(\mathcal{O}_{\mathbb{R}}):P^{*}(\Omega)= P(\Omega)$
2. $\forall\Omega\in\sigma(\mathcal{O}_{\mathbb{R}}):P(\Omega)\circ P(\Omega)=P(\Omega)$
3. $P(\mathbb{R}) = id_H$
4. $\forall\Omega\in\sigma(\mathcal{O}_{\mathbb{R}}): \Omega = \dot{\bigcup}_{n\geq 1}\Omega_n\implies \forall\psi\in H:\sum_{\geq 1}(P(\Omega_n)\Psi)=P(\Omega)\psi$ where $\Omega_n\cap\Omega_m = \emptyset$.

*Properties:* If $P$ is a PVM then 
1. $P(\emptyset)= \text{null}:H\rightarrow H$ where $H\ni\psi\mapsto 0_H$.
2. $P(\mathbb{R}\backslash\Omega) = id_H-P(\Omega)$ for any $\Omega\in\sigma(\mathcal{O}_\mathbb{R})$
3. $P(\Omega_1\cup\Omega_2)+P(\Omega_1\cap\Omega_2)=P(\Omega_1)+P(\Omega_2)$
4. $P(\Omega_1\cap\Omega_2)=P(\Omega_1)\circ P(\Omega_2)$
5. $\Omega_1\subseteq\Omega_2\implies \text{ran}(P(\Omega_1))\subseteq \text{ran}(P(\Omega_2))$.

Proof:



*Remark* it suffices to know $P((-\infty,\lambda])\forall \lambda\in\mathbb{R}$. Therefore we define $P((-\infty,\lambda])=:P(\lambda)$.