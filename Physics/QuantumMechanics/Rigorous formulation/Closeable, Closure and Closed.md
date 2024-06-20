---
aliases: [closable, closure, closed]
---
*Definitons:* 
1. A densely defined operator $A$ is called ***closable*** it its adjoint $A^*$ is also densely defined.
2. The ***closure*** of a closable operator $A$ is defined as $$\overline{A} = A^{**}.$$
3. An operator $A$ is called closed if $A = \overline{A}$.


### Example
Symmetric operator $A$ is always closable
*Proof:*  We have to show that $\mathcal{D}_A^*$ is also densely defined. We know that symmetry of $A$ implies $A\subseteq A^*$ by [[Symmetric operator|theorem]]. This means $\mathcal{D}_A\subseteq\mathcal{D}_{A^{*}}\implies \overline{\mathcal{D}}_A \subseteq \overline{\mathcal{D}}_{A^{*}}$  which is topologically closed. This means $H = \overline{\mathcal{D}}_A \subseteq \overline{\mathcal{D}}_{A^{*}}\subseteq H\implies \overline{D}_{A^*} = H$.