---
aliases: [proposition about equipotent sets]
---

#SetTheory 

*Proposition:* Let $A$, $B$ and $C$ be sets.
1. Then $A$~$A$.
2. If $A$~$B$ then $B$~$A$.
3. if $A$~$B$ and $B$~$C$ then $A$~$C$.

*Proof:* 
1. The identity function $f(x) = x$ for $x\in A$ is a bijection.
2. If $f$ is a bijection from $A$ to $B$, then its inverse $g$ is a bijection from $B$ to $A$.
3. If $f$ is a bijection from $A$ to $B$ and $g$ is bijection from $B$ to $C$ then $g\circ f$ is a bijection from $A$ to $C$.

This proposition shows that "~" is 1. reflexive, 2. symmetric and 3. transitive; that is, "~" is a equivalence relation.

