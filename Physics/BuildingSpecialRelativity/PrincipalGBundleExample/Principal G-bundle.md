## Definiton
*Definiton:* A smooth fibre bundle $(E,\pi,M,F)$ is called a *principal G-bundle* if 
1. $E$ is a [[Right G-action|right G-space]]
2. The right $G$-action $\triangleleft$ is [[Right G-action#Stablizers|free]]
3. There is a bundle-morphism between $E\stackrel{\pi}{\longrightarrow}M$ and $E\stackrel{\rho}{\longrightarrow}E\backslash G$ 
where $E\backslash G$ is a *quotient space*.

### Defining the Principal G-bundle quotient space
We focus on defining the quotient space $E\backslash G$. To do this we look at [[Right G-action#Orbitals|orbitals]] for all $p\in E$ and define an *equivalence relation* ~ the points. The equivalence relation has the following definiton
$$
 p\sim q \iff: p\in\mathit{O}_q
$$
So we say that $p\sim q$ if there exists a $g\in G$ such that $q\triangleleft g = p$. This is an equivalence relation since it is 
1. Reflexive: $q\sim q$
2. Symmetry: $p\sim q\implies  q\sim p$
3. Transitive: $p\sim q \land q\sim r \implies p\sim r$.

Using the equivalence relation we can then create the quotient space 
$$
E\backslash \sim :=\{\mathit{O}_p: p\in E\}.
$$
We have to choose which orbitals we put in this set since $p\in\mathit{O}_{q}\implies q\in\mathit{O}_{p}$. We define 
$$
E\backslash G:= E\backslash\sim.
$$

### Defining the projection from total space to the quotient space

We define $\rho: E\longrightarrow E\backslash G$ as 
$$
\forall p\in E:\rho(p):= \mathit{O}_q\quad\text{where } p\in\mathit{O}_q.
$$
So we take a point and place it into an orbital it belongs to. 
