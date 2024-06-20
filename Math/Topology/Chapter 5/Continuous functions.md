---
	aliases: [continuous functions]
---

In real analysis we define a function $f:\mathbb{R}\rightarrow\mathbb{R}$ to be **countinous** if for each $a\in \mathbb{R}$ and each $\epsilon > 0$ there exists $\delta>0$ such that 
$$
\forall x\in |x-a|<\delta\implies |f(x)-f(a)|<\epsilon.
$$
We may rewrite this definiton in terms of intervals
$$
\forall a\in\mathbb{R},\forall \epsilon>0\exists\delta>0:\forall x\in(a-\delta,a+\delta)\implies f(x)\in(f(a)-\epsilon,f(a)+\epsilon).
$$
However we want to write this definition in the language of topology i.e. in terms of open sets.

### Lemma 1
*Lemma 1:* Let $f:\mathbb{R}\rightarrow\mathbb{R}$. Then $f$ is continous if and only if for each $a\in\mathbb{R}$ and each open set $U$ containing $f(a)$ there exists open set $V$ such that it contains $a$ and $f(V)\subseteq U$.

*Proof:* Suppose $f$ is continous. Then by definiton 
$$
\forall a\in\mathbb{R},\forall \epsilon>0\exists\delta>0:\forall x\in(a-\delta,a+\delta)\implies f(x)\in(f(a)-\epsilon,f(a)+\epsilon).
$$
Set $V=(a-\delta,a+\delta)$ and $U=(f(a)-\epsilon,f(a)+\epsilon)$. Then for each $a\in\mathbb{R}$ and each open set $U$ containing $f(a)$ there exist open set $V$ containing $a$ such that $f(V)\subseteq U$.

Conversely assume for each $a\in\mathbb{R}$ and each open set $U$ contaning $f(a)$ there exists open set $V$ contaning $a$ such that $f(V)\subseteq U$. Choose $U=(f(a)-\epsilon,f(b)+\epsilon)$. Then by assumption there exists open set $V$ containing $a$ such that $f(V)\subseteq U$. As $V$ is an open set contaning $a$ there exists $c,d$ such that $a\in(c,d)\subseteq V$. Set $\delta = \text{min}(a-c,d-a)$. Then create $(a-\delta,a+\delta)$. Clearly $(a-\delta,a+\delta)\subseteq V$. Therefore we have found a $\delta>0$ for each $a\in\mathbb{R}$ and $\epsilon>0$ $\forall x\in(a-\delta,a+\delta)\implies f(x)\in(f(a)-\epsilon,f(a)+\epsilon)$.


### Lemma 2

*Lemma 2*: Let $f$ be a mapping from topological space $(X,\tau)$ into a topological space $(Y,\tau')$. Then the following two conditions are equivalent:
(i) for each $U\in\tau'$, $f^{-1}(U)\in\tau$;
(ii) for each $a\in X$ and each $U\in\tau'$ with $f(a)\in U$, there exists $V\in\tau$ such that $a\in V$ and $f(V)\subseteq U$.

*Proof:* Assume (i) is true. Let $a\in X$, $U\in\tau'$ with $f(a)\in U$. Then $f^{-1}(U)\in\tau$. Let $V=f^{-1}(U)$. Then we have found $V\in\tau$ such that $a\in V$ and $f(V)\subseteq U$.

Assume (ii) is true. Then we take $U\in\tau'$. If $f^{-1}(U)=\emptyset$ then $f^{-1}(U)\in\tau$. Suppse $f^{-1}(U)\neq\emptyset$. Let $a\in f^{-1}(U)$. Then $f(a)\in U$.  By assumption there exists $V\in\tau$ such that $f(V)\subseteq U$. This means for each $a\in f^{-1}(U)$ there exists $V\in\tau$ such that $a\in V\subseteq f^{-1}(U)$. By corollary [[Open sets and open sets|open sets and open sets]] $f^{-1}(U)\in\tau$.


### Definiton

*Definiton:* Let $(X,\tau)$ and $(Y,\tau')$ be topological spaces. Then $f:(X,\tau)\rightarrow(Y,\tau')$ is said to be **continous** if for each $U\in\tau',f^{-1}(U)\in\tau$.






