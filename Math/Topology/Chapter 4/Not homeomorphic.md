---
aliases: [not homeomorphic]
---

We have defined what it means for two topologies to be [[Homeomorphism|homeomorphic]]. Now we try find techniques that will help us check if two topologies are not homeomorphic. 

E.g. Prove $[0,2]$ is not homeomorphic to the subspace $[0,1]\cup[2,3]$ of $\mathbb{R}$.

Let $(X,\tau)=[0,2]$ and $(Y,\tau_1)=[0,1]\cup[2,3]$. Then we can see that $Y\backslash [0,1]=[2,3]$ which is an [[Open and Closed sets|open set]] of $\tau_1$. Furthermore, $Y\backslash[2,3]=[0,1]$ which is an open set of $\tau_1$. Therefore we have found a proper non empty clopen subset of $Y$. Therefore $(Y,\tau_1)$ is not a [[Math/Topology/Connected|connected]] space. 

However, $(X,\tau)$ is a connected space.

Suppose that a [[Homeomorphism|homeomorphism]] exists between $(X,\tau)$ and $(Y,\tau_1)$. Then $f:X\rightarrow Y$. Now take a subset $[0,1]\subseteq Y$. Then $f^{-1}([0,1])\in\tau$. This means there exists a proper non emty clopen subset of $X$. Which implies that $X$ is not connected. This is a contradiction. $(X,\tau)\ncong(Y,\tau_1)$. 

