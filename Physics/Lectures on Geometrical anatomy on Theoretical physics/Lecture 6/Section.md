---
aliases: [section]
---

*Definition:* Let $E\stackrel{\pi}{\rightarrow}M$ be a [[Physics/Lectures on Geometrical anatomy on Theoretical physics/Lecture 6/Bundles|bundle]]. A map $\sigma:M\rightarrow E$ is called a **section** of the bundle if 
$$
\pi\circ\sigma=\text{id}_M.
$$
The intuition behind this definiton is as follows: Take any point $p$ from base space $M$. We are free to define a map $\sigma$ that takes $p$ and maps it to any point $q$ in total space $E$. However if the projection of $q$ i.e. $\pi(q)\neq p$ then $\sigma$ is not a section. 

For sigma to be a section it must map $p\in M$ to a $r\in E$ such that $\pi(r) = p$.

### Representing a section as a function
Let $E\stackrel{\pi}{\rightarrow}M$ be a bundle where $E = M\times F$. Then we may define a section $\sigma$ as 
$$
\begin{aligned}
\sigma:M&\rightarrow M\times F\\
p&\mapsto (p,s(p))\\
\text{where } s:M&\rightarrow F.
\end{aligned}
$$
So $s$ is a map take takes point $p\in M$ and only maps it to a point in the [[Fiber|fiber]] $F$ that is attached at point $p$.

We can talk about a physical example. Suppose we have a $\mathbb{C}$ line bundle over $M$. That is $\forall p\in M$, $\mathbb{C}$ is attached. Then the wavefunction in quantum mechanics is a section of the $\mathbb{C}-$line bundle over physical space.


