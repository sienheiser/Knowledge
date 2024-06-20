---
aliases: [Gross-Piteavski equation, GPe]
---
#MasterThesis

### GPe equation

The GPe equation is the following

$$
i\hbar\frac{\partial \Psi}{\partial t} = [-\frac{\hbar^2}{2m}\nabla^2+V(\vec{r})+U|\Psi|^2]\Psi
$$
where $\Psi$ is the wavefunction, $V$ is the trap potential, $U$ is the scattering potential.

### Derivation of GPe equation
Suppose we have a system with $N$ interacting particles in an external trap. The Hamiltonian for such a system is

$$
\hat{\mathcal{H}} = \sum_{i=1}^N\frac{\hat{p_i}^2}{2m}+\hat{V}_{ext}(\vec{r}) + \frac{1}{2}\sum_{i=1}^N\sum_{j\neq i}^N\hat{V}(\vec{r}_i-\vec{r}_j).
$$
There is a half before the last sums because the two sums double count all the interaction between each pair of particles. To see this suppose we take $i=1$ and run over $j = 2$ to $j=N$. Then take $i=2$ and run over $j = 1,3,4,....,N$. Notice we have double counted the $V(\vec{r}_1-\vec{r}_2)$. When we take $i = 3$ and $j = 1,2,4,....,N$ then we would double count $V(\vec{r}_1-\vec{r}_3)$ and $V(\vec{r}_2-\vec{r}_3)$. This keeps going on untill all the interaction have been double counted.

The ground state corresponds to minimum energy of the Hamiltonian. To find the minimum we can use the [[Free energy]] $F = E-\mu N$ ***(why do we use the free energy?)*** where $E$ is the energy, $\mu$ is the [[chemical potential]] and  $N$ is the number of particles in the system. Given a Hamiltonian $\mathcal{H}$ and a wavefunction $|\psi>$ the energy is obtained by 
$$
E(\psi) = \frac{<\psi|\mathcal{H}|\psi>}{<\psi|\psi>}.
$$
In the condensate we have $N$ particles, meaning that each particle has its own wavefunction $\psi_i$. However, if the particles are far away from each other then we can do a mean field approximation. Essentially, we say that all the individual wave functions are the same ***why?***. This means that the state ket has form $|\Psi> = |\psi>\otimes....\otimes|\psi>$, where $\otimes$ is the tensor product. The normalization for the state ket is taken to be unity. The problem is reduced to minimizing $F(\Psi)= <\Psi|\hat{\mathcal{H}}|\Psi>-\mu <\Psi|\Psi>$ ***Something wrong with the equation. Where did the $N$ go?. Is the normalization of state ket not unity?***.

The kinetic energy term reads as

$$
<\Psi|\sum_{i=1}^N\frac{\hat{p_i}^2}{2m}|\Psi> = \sum_{i=1}^N\frac{\hbar^2}{2m}\int \nabla\psi^*(\vec{r}_i)\nabla\psi(\vec{r}_i)d\vec{r}_i.
$$
where $|\Psi>$ is the $N$ particle state ket and $\psi(\vec{r})$ is the single particle wave function.
***Not sure why we add over all the single particle wavefunctions. Is it because the ith momentum operator only works on the ith single particle wavefunction? If so then what happens to the remaining single particle wavefunction? *** 
Since all the single particle wavefunctions are the sum we replace the sum with $N$ giving

$$
<\Psi|\sum_{i=1}^N\frac{\hat{p_i}^2}{2m}|\Psi> = N\frac{\hbar^2}{2m}\int \nabla\psi^*(\vec{r})\nabla\psi(\vec{r})d\vec{r}.
$$

Using [[Green's identity]] we can rewrite the integral as 
$$
N\frac{\hbar^2}{2m}\int \nabla\psi^*(\vec{r})\nabla\psi(\vec{r})d\vec{r} = -N\frac{\hbar^2}{2m}\int \psi^*(\vec{r})\nabla^2\psi(\vec{r})d\vec{r}.
$$
The external potential term is written as
$$
<\Psi|\hat{V}_{ext}(\vec{r})|\Psi> = N \int\psi^*(\vec{r})V_{ext}\psi(\vec{r})d\vec{r}.
$$
***I am guessing the N comes from the N single wave function in $\Psi$***.

The interaction term becomes
$$
<\Psi|\frac{1}{2}\sum_{i=1}^N\sum_{j\neq i}^N\hat{V}(\vec{r}_i-\vec{r}_j)|\Psi> = \frac{1}{2}\sum_{i=1}^N\sum_{j\neq i}^N\int d\vec{r}_i\int d\vec{r}_j \psi^*(\vec{r}_i)\psi^*(\vec{r}_j)V(|\vec{r}_i-\vec{r}_j|)\psi(\vec{r}_i)\psi(\vec{r}_j).
$$
Since all the individual wavefunctions are the same we are adding the the same wave function $N(N-1)/2$ times giving

$$
<\Psi|\frac{1}{2}\sum_{i=1}^N\sum_{j\neq i}^N\hat{V}(\vec{r}_i-\vec{r}_j)|\Psi> = \frac{N(N-1)}{2}\int d\vec{r}\int d\vec{r}^{'} \psi^*(\vec{r})\psi^*(\vec{r}^{'})V(|\vec{r}-\vec{r}^{'}|)\psi(\vec{r})\psi(\vec{r}^{'}).
$$
Finally the last term is

$$
\mu<\Psi|\Psi> = \mu\left(\int \psi^*(\vec{r})\psi({\vec{r}})d\vec{r}\right)^N.
$$
Using the [[variational principle]] we can minimize the Free energy. We can rewrite the free energy as a sum of functionals

$$
F(\psi,\psi^*) = J_1(\psi,\psi^*) +J_2(\psi,\psi^*) +J_3(\psi,\psi^*) + J_4(\psi,\psi^*).
$$

Taking  the [[functional derivative|functional derivative]] of the entire expression w.r.t to $\psi^*$ gives 
$$
\frac{d}{d\epsilon}F(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0} = \frac{d}{d\epsilon}J_1(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0} +\frac{d}{d\epsilon}J_2(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0} +\frac{d}{d\epsilon}J_3(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0} + \frac{d}{d\epsilon}J_4(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0}.
$$
The functional derivative of $J_1$ is

$$
\frac{d}{d\epsilon}J_1(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0}  = -N\frac{\hbar^2}{2m}\int \frac{d}{d\epsilon}(\psi^*(\vec{r})+\epsilon\eta(\vec{r}))\nabla^2\psi(\vec{r})d\vec{r}= -N\frac{\hbar^2}{2m}\int \eta(\vec{r})\nabla^2\psi(\vec{r})d\vec{r}.
$$

The functional derivative of $J_2$ is 
$$
\frac{d}{d\epsilon}J_2(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0} =N \frac{d}{d\epsilon}\int(\psi^*(\vec{r})+\epsilon\eta(\vec{r}))V_{ext}\psi(\vec{r})d\vec{r} = \int\eta(\vec{r})V_{ext}\psi(\vec{r})d\vec{r}.
$$
The functional derivative of $J_3$ is

$$
\frac{d}{d\epsilon}J_3(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0}  = \frac{N(N-1)}{2}\frac{d}{d\epsilon}\int \int  \left[\psi^*(\vec{r})+\epsilon\eta(\vec{r})\right] \left(\psi^*(\vec{r}^{'})+\epsilon\eta(\vec{r}^{'})\right)V(|\vec{r}-\vec{r}^{'}|)\psi(\vec{r})\psi(\vec{r}^{'})d\vec{r}d\vec{r}^{'}.
$$
In this case we will have to use the product rule. Therefore the term $\frac{d}{d\epsilon}\left[\psi^*(\vec{r})+\epsilon\eta(\vec{r})\right] \left(\psi^*(\vec{r}^{'})+\epsilon\eta(\vec{r}^{'})\right)|_{\epsilon = 0}=\eta(\vec{r})\psi^*(\vec{r}^{'})+\psi^*(\vec{r})\eta(\vec{r}^{'})$. This gives 

$$
\frac{d}{d\epsilon}J_3(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0}  = \frac{N(N-1)}{2}\int  \left(\eta(\vec{r})\psi^*(\vec{r}^{'})+\psi^*(\vec{r})\eta(\vec{r}^{'})\right)V(|\vec{r}-\vec{r}^{'}|)\psi(\vec{r})\psi(\vec{r}^{'})d\vec{r}d\vec{r}^{'}
$$
$$
\implies \frac{d}{d\epsilon}J_3(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0}  = \frac{N(N-1)}{2}\int  \left(\eta(\vec{r})|\psi(\vec{r}^{'})|^2V(|\vec{r}-\vec{r}^{'}|)\psi(\vec{r})+|\psi(\vec{r})|^2\eta(\vec{r}^{'})V(|\vec{r}-\vec{r}^{'}|)\psi(\vec{r}^{'})\right)d\vec{r}d\vec{r}^{'}.
$$
The two integrals are the same if we rename the radius vectors of one them (***This can be done because boson wave functions are symmetric***). This gives
$$
\frac{d}{d\epsilon}J_3(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0}  = N(N-1)\int  \left(|\psi(\vec{r}^{'})|^2V(|\vec{r}-\vec{r}^{'}|)\psi(\vec{r})\eta(\vec{r})\right)d\vec{r}d\vec{r}^{'}.
$$
Finally $J_4$ becomes 
$$
\frac{d}{d\epsilon}J_4(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0} =-\mu \frac{d}{d\epsilon}\left(\int \left[\psi^*(\vec{r})+\epsilon\eta(\vec{r})\right]\psi({\vec{r}})d\vec{r}\right)^N|_{\epsilon = 0}.
$$
Here we use the product rule $N$ times which gives

$$
\frac{d}{d\epsilon}J_4(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0} =N\int\eta(\vec{r})\psi({\vec{r}})d\vec{r}\left(\int \psi^*(\vec{r})\psi({\vec{r}})d\vec{r}\right)^{N-1} =N\int\eta(\vec{r})\psi({\vec{r}})d\vec{r}
$$
where the last equality comes from the fact that $\int \psi^*(\vec{r})\psi({\vec{r}})d\vec{r}=1$. 

To minimise the free energy we set $\frac{d}{d\epsilon}F(\psi,\psi^*+\epsilon\eta)|_{\epsilon = 0} = 0$. As a result, the final expression is 
$$
0 = N \int \left(-\frac{\hbar^2}{2m}\nabla^2\psi(\vec{r})+V_{ext}(\vec{r})\psi(\vec{r})+(N-1)\int|\psi(\vec{r}^{'})|^2V(|\vec{r}-\vec{r}^{'}|)d\vec{r}^{'}\psi(\vec{r}) - \mu\psi(\vec{r})\right)\eta(\vec{r})d\vec{r}.
$$

Since $\eta$ is an arbitrary function the expression in the brackets must equal zero giving
$$
-\frac{\hbar^2}{2m}\nabla^2\psi(\vec{r})+V_{ext}(\vec{r})\psi(\vec{r})+(N-1)\int|\psi(\vec{r}^{'})|^2V(|\vec{r}-\vec{r}^{'}|)d\vec{r}^{'}\psi(\vec{r}) - \mu\psi(\vec{r}) = 0
$$




