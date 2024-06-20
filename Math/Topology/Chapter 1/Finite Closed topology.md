---
aliases: [finite closed topology, cofinite topology]
---

*Definiton:* Let $X$ be any non-empty set. A topology $\tau$ on $X$ is called a **finite closed topology** or **cofinite topology** if the closed subsets of $X$ are $X$ and its finite subsets.

*Remark* We have not spoken about $X$ being finite or infinite. It can be either. But if $X$ is infinite do not fall in the trap and assume every infinite subets of $X$ is an [[Open and Closed sets|open set]]. Example $X = \mathbb{N}$ then can make set of all even numbers. But this set is not closed in the cofinite topology meaning the set of all odd numbers is not an open set.

*Remark* If $(X,\tau)$ is a finite closed topological space and $X$ has atleast three clopen subsets then $X$ is a finite set.
*proof:* We know from the [[Proposition for open and closed sets|proposition for closed sets]] that $X$ and $\emptyset$ are always closed sets. Meaning there is one other clopen set $S$. Since it is a closed set it is a finite set because we are in a cofinite topology. Since it is a open set we know $X\backslash S$ is a closed set and therefore also a finite set. But $S\cup X\backslash S=X$. Since $X$ is the union of two finite sets it is a finite set.