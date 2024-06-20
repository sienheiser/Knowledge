---
aliases: [homeomorphism, homeomorphic]
---

*Definiton:* Let $(X,\tau)$ and $(Y,\tau_1)$ be topological spaces. Then they are said to be **homeomorphic** if there exists a function $f: X\rightarrow Y$ which has the following properties:
(i) f is [[Injective, Surjective and Bijective|injective]],
(ii) f is [[Injective, Surjective and Bijective|surjective]],
(iii) for each $U\in \tau_1$, $f^{-1}(U)\in\tau$, and 
(iv) for each $V\in\tau$, $f(V)\in\tau_1$.

Further, the map $f$ is said to be a **homeomorphism** between $(X,\tau)$ and $(Y,\tau_1)$. We write $(X,\tau)\cong (Y,\tau_1)$. 

The relation $\cong$ is an equivalence relation.

*Proof:* We will show that it is transitive. Let $(X,\tau)$, $(Y,\tau_1)$ and $(Z,\tau_1)$ homeomorphic. Then there exists homeomorphisms $f,g$ such that $f:X\rightarrow Y$ and $g:Y\rightarrow Z$. The composition $g\circ f$ is [[Injective, Surjective and Bijective|bijective]] ( #ToBeProven ). Now take any $U\in \tau_2$. Then $g^{-1}(U)\in \tau_1$ and $f^{-1}(g^{-1}(U))\in\tau$. Also take any $V\in\tau$ then $f(V)\in\tau_1$ and $g(f(V))\in\tau_2$. So the composition has properties (iii) and (iv). 

In a similar fashion, $\cong$ can be shown to be reflexive and transitive.

