---
aliases: [subspace topology, subspace, relative topology, induced topology]
---

*Definition:* Let $Y$ be a non-empty subset of a [[Axioms|topological space]] $(X,\tau)$. The collection $\tau_Y=\{O\cap Y|O\in\tau\}$ is a topology on $Y$ called the **subspace topology**. The topological space $(Y,\tau_Y)$ is said to be a **subspace** of $(X,\tau)$. 

*Proof:* We show that $\tau_Y$ is a topology.

(i) Since $\emptyset\in\tau$ and $\emptyset\cap Y=\emptyset$ then $\emptyset\in\tau_Y$. Since $X\in\tau$ and $X\cap Y= Y$ then $Y\in\tau_Y$.
(ii) Want to show that the intersection between any two open sets belonging to $\tau_Y$ is an open set belonging to $\tau_Y$. Take $U_y,V_y\in\tau_Y$. There exists $U,V\in\tau$ such that $U_y=U\cap Y$ and $V_y = V\cap Y$. Now $U_y\cap V_y = (U\cap Y)\cap(V\cap Y) = (U\cap V)\cap Y$. Since $U\cap V\in\tau$ then $U_y\cap V_y\in\tau_Y$.
(iii) #ToBeProven 

