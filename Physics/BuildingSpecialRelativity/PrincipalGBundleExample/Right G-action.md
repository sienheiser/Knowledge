
## Definiton
*Definiton:* Let $G$ be a Lie group and $M$ a smooth manifold

Then 
$$
\triangleleft:M\times G\rightarrow M
$$
is called a right $G$-aciton on M if

1. $\forall p\in M:p\triangleleft e=p$ where $e\in G$ is the identity
2. $\forall g_1,g_2\in G:\forall p\in M:(p\triangleleft g_1)\triangleleft g_2 = p\triangleleft(g_1\cdot g_2)$ 

We then call $M$ a right $G$-space.

### Stablizers
For all points $p\in M$ we can define the set 
$$
S_p = \{g\in G:p\triangleleft g=p\}.
$$
We call the $S_p$ the stablizer of $p$. If $$\forall p\in M:S_p = \{e\}$$ where $e\in G$ is the identity. Then the right action is *free*.

### Orbitals
For all point $p\in M$ we can define the set
$$
\mathit{O}_p = \{q\in M:\exists g\in G:p\triangleleft g=q\}.
$$
That is if there is $g\in G$ such that $g$ acting on $p$ produces $q\in M$ then $q$ belongs to $\mathit{O}$. 