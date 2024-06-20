---
aliases: [virial theorem]
---
#ClassicalMechanics 

The Virial theorem relates the time average of the kinetic energy of a system to a time average of the potential energy of the same system. 

### Virial theorem
We know that the kinetic energy term in the Lagrangian is a quadratic function of vecocity. This means that if a system has multiple particles the following is true

$$
2 T = \sum_a \frac{\partial T}{\partial \vec{v}_a}\cdot \vec{v}_a = \frac{d}{dt}\sum_a \vec{p}_a\cdot \vec{r}_a - \sum_a \dot{\vec{p}}_a \cdot \vec{r}_a, 
$$
where we have used $\frac{\partial T}{\partial \vec{v}} = \vec{p}$ and the product rule. The time average of a function is defined to be 

$$
\bar{f} = \lim_{\tau\rightarrow\infty} \frac{1}{\tau} \int_0^{\tau}f(t)dt.
$$

If $f(t)$ is a total time derivative of a function $F(t)$ then 
$$
\bar{f} = \lim_{\tau\rightarrow\infty} \frac{1}{\tau} \int_0^{\tau}f(t)dt = \lim_{\tau\rightarrow\infty} \frac{1}{\tau} \int_0^{\tau}\frac{d}{dt}F(t)dt = \lim_{\tau\rightarrow\infty}\frac{F(\tau)-F(0)}{\tau}.
$$
If $F(t)$  is a bounded function then the time average is zero. Similarly if we take the time average of the expression for $2T$ then the $\frac{d}{dt}\sum_a \vec{p}_a\cdot\vec{r}_a$ is zero since in a finite space neither the momentum or the radius vector can be infinite in magnitude. If we substitue $\frac{\partial U}{\partial\vec{r}} = \dot{\vec{p}}$  we obtain
$$
2\overline{T} = \overline{\sum_a \vec{r}_a\cdot\frac{\partial U}{\partial \vec{r}_a}}.
$$

If the potential $U$ is a homogenous function of order $k$ w.r.t the radius vector then $\frac{\partial U}{\partial \vec{r}} = kU$. Which means that in general 

$$
2\overline{T} = k\overline{U}.
$$

The total average energy $\overline{E}$ must still equal to the total energy $E$ of the system. This means that $\overline{E} = \overline{T}+\overline{U} = E$. As a result, we obtain the following relations 
$$
\overline{T} = \frac{E}{1+\frac{2}{k}},\quad \overline{U} = \frac{E}{1+\frac{k}{2}}.
$$

### Significance of the Virial theorem

For a normal harmonic oscillator the potential had degree $k=2$. This means $\overline{T} = \overline{U}$ which says that the average kinetic energy and potential are the same. 

In the case of the Newtonian potential, k = -1. This means that $\overline{T} = -\frac{1}{2}\overline{U}$  and the total energy is $E = -\overline{T}$
