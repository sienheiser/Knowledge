*Definiton:* A bundle (of topological manifolds) is a triple $(E,\pi,M)$ where $E$ and $M$ are [[Physics/Lectures on Geometrical anatomy on Theoretical physics/Lecture 6/Manifold|manifolds]]. $E$ is called the **total space**, $M$ is called the **base space** and $\pi$ is a surjective map $\pi:E\rightarrow M$ which is a continous map. $\pi$ is called a projection. 

### Fibres
Suppose we start with a base space $M$. Take any point $p\in M$. Now imagine that we have a projection map $\pi$ such that $\text{preim}_\pi(\{p\})=F_p$, where $F_p$ is some manifold at $p$. Then $F_p$ is known as a **fibre** at $p$. 

For example, let $M, F$ be topological manifolds. Then set $E=M\times F$. If we define projection map 
$$
\begin{aligned}
\pi:M\times F&\rightarrow M\\
(p,f)&\mapsto p
\end{aligned}
$$
where $p\in M$ and $f\in F$. The $\pi$ is continous if $E$ is equipped with the product topology. 

The intuition is as follows, if we have some base space $M$ then we can attach some manifold at each point of $M$. We are free to attach different manifolds at each points of $M$ or the same manifold at each point of $M$. These manifolds that are attached are known as fibres. 

#### Fibre bundle
If we take a base space $M$ and for all $p\in M$ we only attach fibres that are [[Homeomorphism|homeomorphic]] to each other. Then we call this a **fibre bundle**.

More formally
*Definiton:* Let $E\stackrel{\pi}{\rightarrow}M$ be a bundle. If $\forall p\in M:\text{preim}_\pi(\{p\})\cong F$ for some manifold F. Then $E\stackrel{\pi}{\rightarrow}M$, where $E=M\times F$, is known as a **fibre bundle**.

### Sub bundles
 Let $E\stackrel{\pi}{\rightarrow}M$ be a bundle.  Let $E'\stackrel{\pi '}{\rightarrow}M'$ is a subbundle if $E'\subset E$, $M'\subset M$, $\pi'=\{p|p\in E'\}:= \pi |_{E'}$.
### Structures
We know how to make product manifolds. However, fibre bundles are more general than product manifolds. We get the following restrictions product manifolds $\subset$ fibre bundles $\subset$ bundles.





