---
aliases: [basis for topology, basis]
---
*Definiton:*  Let $(X,\tau)$ be a [[Axioms|topological space]]. A collection $\mathcal{B}$ of open subsets of $X$ is said to be a **basis** for the topology $\tau$ if every open set is the union of members of $\mathcal{B}$.

*Example 1:* Let $\mathcal{B}=\{(a,b)|a,c\in\mathbb{R},a<b\}.$ Since $\mathcal{B}$ consists of open intervals $(a,b)$ we know that $(a,b)\in\tau$. Now take and open set $S\in\tau$. By [[Proposition for Euclidean topology on real numbers|proposition for euclidean topology on real numbers]] we know that $S$ must be a union of open intervals. Since all open intervals are members of $\mathcal{B}$, $\mathcal{B}$ must be a basis for [[The Euclidean Topology on Real numbers|euclidean topology on real numbers]].

*Example 2:* Let $(X,\tau)$ be a [[Discrete and indiscrete topology|discrete space]] and $\mathcal{B}=\{\{x\}|x\in X\}$. Then $\mathcal{B}$ is a basis for $\tau$. 

*Example 3:* Let $X = \{a,b,c,d,e,f\}$ and $$\tau_1=\{X,\emptyset,\{a\},\{c,d\}, \{a,c,d\}, \{b,c,d,e,f\}\}.$$ Then $\mathcal{B} = \{\{a\},\{c,d\},\{b,c,d,e,f\}\}$ is a basis for $\tau_1$ as $\mathcal{B}\subseteq \tau_1$ and every memeber of $\tau_1$ can be expressed as a union of members of $\mathcal{B}$. Note that $\tau_1$ itself is also a basis for $\tau_1$. *Note* that $\tau_1$ is a basis for itself.

Suppose that $\mathcal{B}$ is a basis for topology $\tau$ on a set $X$. Let $\mathcal{B}_1$ be a collection of subsets of $X$ such that $\mathcal{B}\subseteq\mathcal{B}_1\subseteq\tau$, then $\mathcal{B}_1$ is also a basis for $\tau$.

*proof:* We know that $\mathcal{B}$ is a basis on topology $\tau$ on set $X$. We have another set $\mathcal{B}_1$ such that $\mathcal{B}\subseteq\mathcal{B}_1\subseteq\mathcal\tau$. Take any member $S_1\in\mathcal{B}_1$, then $S_1$ must either belong to $\mathcal{B}$ or $S_1$ must be a union of members of $\mathcal{B}$ because $\mathcal{B}\subseteq\mathcal{B}_1\implies$ for all $S\in\mathcal{B}$, $S$must belong to$\mathcal{B}_1$ and $\mathcal{B}_1\subseteq\tau$ implies for all $S'\in \mathcal{B}_1$, $S'$ belongs to $\tau$. Take any union of elements members from $\mathcal{B}_1$
$$
\bigcup_{S'\in\mathcal{B}_1}S'
$$
then this union must belong to $\tau$ since $S'\in\mathcal{B}_1$ is either a member of $\mathcal{B}$ which is a basis of $\tau$ or $S'=\bigcup_{S\in\mathcal{B}}S$ which still belongs to $\tau$ because $\mathcal{B}$ is a basis of $\tau$. Therefore, $\mathcal{B}_1$ is a basis of $\tau$.