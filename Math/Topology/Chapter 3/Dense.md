---
aliases: [dense]
---

*Definiton:* Let $A$ be a subset of [[Axioms|topological space]] $(X,\tau)$. Then $A$ is said to be dense in $X$ or everywhere dense in $X$ if $\bar{A} = X$.


E.g The closure of the set of all rational numbers if the real number $\overline{\mathbb{Q}} = \mathbb{R}$. 

*Proof:*  Suppose the $\overline{\mathbb{Q}} \neq \mathbb{R}$. Then we know that $\mathbb{R}\backslash\overline{\mathbb{Q}}$ is an open set that is not an empty set. This means that there is an $x\in\mathbb{R}\backslash\overline{\mathbb{Q}}$, by the definiton of a topology there  must exist an open interval such that
$$
x\in(a,b)\subseteq \mathbb{R}\backslash\overline{\mathbb{Q}}.	
$$
But every open interval contains rational numbers. Since $\mathbb{R}\backslash\overline{\mathbb{Q}}$ cannot contain any rational numbers this is a contradiction. Therefore $\overline{\mathbb{Q}}=\mathbb{R}$.