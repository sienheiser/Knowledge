---
aliases: [ensemble averages]
---

#QuantumMechanics 

We have talked about why the state kets we use cannot cope with systems that have more than one state ket in [[Motivation for Density operator|motivation for density operator]]. Here we introduce the emsemble average of an observable. 


### Ensemble Average

Imagine a system that contains different states that can be represented by state set of state kets $\{|\alpha^{(i)}\rangle, i = 1,.....,n\}$. Note that each state ket $|\alpha^{(i)}\rangle$ can be described in the same ket space (Hilbert Space). For example, we may have a system with 40% in positive spin z direction, 30% in positive spin x direction and 30% in negative spin y direction. The Hilbert space for spin 1/2 system is still two dimensional. ***However the system as whole is not in a superposition of the different states $|\alpha^{(i)}\rangle$*** .

Let us call $w_1$ the fraction of the population that is state $|\alpha^{(1)}\rangle$, $w_2$ the fraction of the the population that is in state $|\alpha^{(2)}\rangle$,....., $w_n$ the fraction of the population that is in state $|\alpha^{(n)}\rangle$. Then by definition the following is true

$$
\sum_{i=1}^n w_i = 1.
$$

Suppose we want to measure some observable $A$ ($A$ can be the usual spin operator). Then to compute the average value of $A$ we must use the ***ensemble average***
$$
[A] = \sum_{i=1}^n w_i\langle\alpha^{(i)}| \hat{A} |\alpha^{(i)}\rangle. 
$$
We may introduce a set of [[basis kets]] which are [[eigenkets]] of operator $\hat{A}$. Which gives 
$$
[A] = \sum_{a'} \sum_{i=1}^n w_i|\langle a'|\alpha^{(i)}\rangle|^2 a',
$$
where $|a'\rangle$ are the basis eigenkets and operator $\hat{A}$ and $a'$ are the eigenvalues. Notice how two probabilistic concepts appear: First, $|\alpha^{(i)}\rangle|^2$ which is the probability to find state $|\alpha^{(i)}\rangle$ in $\hat{A}$ eigenstate $|a'\rangle$. Second, $w_i$ which is the probability to find a state $|\alpha^{(i)}\rangle$ in the mixed ensemble. 