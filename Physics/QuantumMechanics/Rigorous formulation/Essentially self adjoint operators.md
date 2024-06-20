---
aliases: [ESAO]
---
Main idea: If we are given some proposed observable, we have to check whether it is [[Self-adjoint and adjoint|self-adjoint]]. We start developing criteras for looking whether an observable,
*Definiton:* A symmetric operator $A$ is called ***essentially self-adjoint*** if its closure $\overline{A}$ is self-adjoint.

*observe:* self-adjoint $\implies$ essentially self-adjoint.

***Theorem:*** For essentially self adjoint operators there exits a unique self adjoint extenstion.
*Proof:* 
1. Since $A$ is symmetric it is closable which was proven in [[Closeable, Closure and Closed]]. This means $\overline{A}$ exits.
2. $A\subseteq \overline{A} = A^{**}$ by lemma 1 in [[Lemma, corollary and theorems for adjoint operators]].
3. Remains to show $\overline{A}$ is unique self-adjoint extenstion. Suppose there is another self-adjoint extenstion $B$ of $A$ then $A\subseteq B = B^*\stackrel{1}{\implies}B^{**}\subseteq A^*\stackrel{2}{\implies}A^{**}\subseteq B^{***}$. This means $A^{**}\subseteq B^{***}\iff \overline{A}\subseteq B$ where $\stackrel{1}{\implies},\stackrel{2}{\implies}$ are true by proposition 2 in [[Propositions for adjoint operator]] and we see that this a unique extenstion by corollary in [[Symmetric operator]].

*Remark:* If operator not essentially self adjoint then either no extention or several extenstions.

