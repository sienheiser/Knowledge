---
aliases: [density operater, density matrix]
---
#QuantumMechanics 


We talked about the [[Ensemble Averages|ensemble averages]]. We can define the density operator from the ensemble average.

### Defining Density Operator
The ensemble average of an observable can be written as 
$$
[A] = \sum_{i=1}^n w_i\langle\alpha^{(i)}| \hat{A} |\alpha^{(i)}\rangle,
$$
where  $|\alpha^{(i)}\rangle$ is the $i$th state in a mixed ensemble and $w_i$ is the fraction of the population of the ensemble in state $|\alpha^{(i)}\rangle$. If we introduce the eigenkets of $\hat{A}$ we get 

$$
[A] = \sum_{i = 1}^n \sum_{b'}\sum_{b''} w_i\langle\alpha^{(i)}| b'\rangle \langle b'|\hat{A} |b''\rangle \langle b''|\alpha^{(i)}\rangle = \sum_{b'}\sum_{b''}   \left(\sum_{i = 1}^n w_i\langle b''|\alpha^{(i)}\rangle\langle\alpha^{(i)}| b'\rangle \right)   \langle b'|\hat{A} |b''\rangle.
$$
We are motivated to define the density matrix $\hat{\rho}$ as 

$$
\hat{\rho} = \sum_{i = 1}^n w_i|\alpha^{(i)}\rangle\langle\alpha^{(i)}|. 
$$

The elements of the matrix can be obtained as

$$
\langle b'|\hat{\rho}|b''\rangle = \sum_{i = 1}^n w_i\langle b'|\alpha^{(i)}\rangle\langle\alpha^{(i)}|b''\rangle.
$$
With the density operator defined as such, we can rewrite the ensamble average as 
$$
[A] = \sum_{b'}\sum_{b''} \langle b''|\hat{\rho}|b'\rangle    \langle b'|\hat{A}|b''\rangle = \text{tr}(\hat{\rho}\hat{A}).
$$
where tr() is known as the [[Trace|trace]].  


