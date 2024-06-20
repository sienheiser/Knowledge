---
aliases: [conditions for a basis to satisfy]
---

*proposition:* Let $X$ be a non-empty set and let $\mathcal{B}$ be a collection of subsets of $X$. Then $\mathcal{B}$ is a basis for a topology on $X$ if and only if $\mathcal{B}$ has the following properties:
1. $X=\bigcup_{B\in\mathcal{B}}$, and
2. for any $B_1,B_2\in\mathcal{B}$, the set $B_1\cap B_2$ is a union of members of $\mathcal{B}$. 

*proof:* Assume that $\mathcal{B}$ is a [[Basis for topology|basis]] for a topology $\tau$ then $\tau$ must satisfy the [[Axioms|axioms]]. Therefore 
$$
X = \bigcup_{S\in\mathcal{B}}S
$$
because $\mathcal{B}$ is a basis for $\tau$ which [[Basis for topology|by definition]] means that every member of $\tau$ is a union of members from $\mathcal{B}$. So property 1 is satisfied. 

Take any two members $T_1,T_2\in\tau$ then $T_1\cap T_2\in\tau$ because $\tau$ is a topology. Since $\mathcal{B}$ is a basis for $\tau$ the two members may be written as 
$$
\begin{aligned}
T_1 &\stackrel{1}{=} \bigcup_{j\in J} B_j\\
T_2 &\stackrel{1}{=} \bigcup_{k\in K} B_k\\
T_1\cap T_2 &\stackrel{1}{=} \bigcup_{i\in I} B_i\\
\end{aligned}
$$
where $J$, $K$ and $I$ are index sets for some $B_j\in\mathcal{B}$, $B_k\in\mathcal{B}$ and $B_i\in\mathcal{B}$. $\stackrel{1}{=}$ is true because all these members of $\tau$ can be represented as unions of members of $\mathcal{B}$. Therefore we have 

$$
\bigcup_{i\in I} B_i= \bigcup_{j\in J} B_j\cap\bigcup_{k\in K} B_k \stackrel{2}{=} \bigcup_{j\in J,k\in K}(B_j\cap B_k)
$$
where $\stackrel{2}{=}$ because of how intersections and unions work. On the one side we have just unions of members of $\mathcal{B}$, on the other side we have unions of intersection between members of $\mathcal{B}$. The only way these can be equal is if the intersection between any two members of $\mathcal{B}$ is a union between memebers of $\mathcal{B}$.

Now we assume that properties mentioned for set $\mathcal{B}$ are true and that $\tau$ has members that are union of members of $\mathcal{B}$. By property 1, $X\in\tau$. Furthermore, $\emptyset\in\tau$ because the emty union between the members of $\mathcal{B}$ can be taken. Therefore $\tau$  satisfied the first [[Axioms|axiom]].
