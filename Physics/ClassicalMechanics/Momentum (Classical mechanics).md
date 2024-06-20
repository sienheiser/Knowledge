---
aliases: [momentum, momentum conservation, Newton's third law]
---
#ClassicalMechanics 


### Momentum
If we move an entire system from one spot to another spot in space. The mechanical properties of the system remain the same. This is due to the space being homogenous (see [[Galileo's Relativity Principle]]). The main idea is to translate the entire mechanical system by an infinitesimal amount $\vec{\epsilon}$.  Suppose the system has Lagrangian $\mathcal{L}(\vec{r})$ with multiple particles. After moving the entire system by $\vec{\epsilon}$ the Lagrangian becomes $\mathcal{L}(\vec{r}+\vec{\epsilon})$. To visualize what is happening here imagine a Cartesian coordinate system describing the system of multiple particles (maybe they interact with each other, maybe not). By adding $\vec{\epsilon}$ to the entire system we shift the entire system. However, we still have the same coordinate system. 

Let us Taylor expand to first order the new Lagrangian at $\vec{\epsilon}=0$. This gives

$$
\mathcal{L}(\vec{r}+\vec{\epsilon}) = \mathcal{L}(\vec{r}) + \sum_a\frac{\partial\mathcal{L}(\vec{r_a}+\vec{\epsilon})}{\partial(\vec{r_a}+\vec{\epsilon})}|_{\vec{\epsilon}= \vec{0}} \frac{d(\vec{r_a}+\vec{\epsilon})}{d\vec{\epsilon}}\cdot \vec{\epsilon} = \mathcal{L}(\vec{r})+\sum_a\frac{\partial\mathcal{L}(\vec{r_a})}{\partial\vec{r_a}}\cdot\vec{\epsilon}.
$$

This implies that

$$
\delta\mathcal{L} = \sum_a\frac{\partial\mathcal{L}(\vec{r_a})}{\partial\vec{r_a}}\cdot\vec{\epsilon}.
$$

Due to the fact that space is homogenous the two Lagrangians are the same. Therefore $\delta\mathcal{L} = 0$ meaning that $\sum_a\frac{d\mathcal{L}(\vec{r_a})}{d\vec{r_a}}\cdot\vec{\epsilon} = 0 = \sum_a \frac{d}{dt}\frac{\partial \mathcal{L}}{\partial \vec{v}_a} =\frac{d}{dt}\sum_a \frac{\partial \mathcal{L}}{\partial \vec{v}_a}$ This means that $\sum_a \frac{\partial \mathcal{L}}{\partial \vec{v}_a}$ is conserved. We define the total momentum of the system to be 

$$
\vec{P} = \sum_a \frac{\partial \mathcal{L}}{\partial \vec{v}_a}.
$$

Note that momentum is also conserved under an external field. Example, if the field points along the z-direction only. Then the x and y momenta are conserved.

### Newton's third law

Notice we have shown that $\sum_a\frac{d\mathcal{L}(\vec{r_a})}{d\vec{r_a}}= 0$. This is the same as $\sum_a F_a = 0$ where $F_a$ is the force on the $a^{\text{th}}$ particle. This is Newton's third law generalized.

### generalized momenta and generalized forces
Genralized momentum is defined to be $\frac{\partial\mathcal{L}}{\partial \dot{q}_i} = p_i$. The generalized force is defined to $\dot{p_i} = F_i$.

In Cartesian coordinates the generalized momenta are components of the vectors $\vec{p_a}$. In general, the $p_i$ are linear [[homogenous function|homogenous functions]]  of genralized velocities $\dot{q}_i$ and do not reduce to products of mass and velocity.