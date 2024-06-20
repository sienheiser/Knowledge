---
aliases: [Euler-Lagrange Equations,EL-equations,ELE, equations of motion]
---
#ClassicalMechanics
#### Derivation of EL-equations
Suppose we have [[Generalized Coordiantes|generalized coordinates]] $q(t)$ such that the [[Principle of Least Action|action]]
$$
S = \int_{t_1}^{t_2} \mathcal{L}(q,\dot{q})dt
$$
is at its least value. Then using [[variational principle]], we can find the differential equation that the generalized coordinates satisfy. 

Suppose we have function $f(t)$ with property $f(t_1) = f(t_2)=0$ . Then define $q(t;\alpha) = q(t)+\alpha f(t)$ where $\alpha$ is a small parameter. The value of $S$ increases with the new generalized cooridnates. If we vary the action w.r.t $\alpha$ then

$$
\frac{\text{d}S}{\text{d}\alpha}|_{\alpha = 0} = \frac{\text{d}}{\text{d}\alpha} \int_{t_1}^{t_2} \mathcal{L}(q(t;\alpha),\dot{q}(t;\alpha))dt=\int_{t_1}^{t_2}\frac{\partial\mathcal{L}}{\partial q}f+\frac{\partial\mathcal{L}}{\partial \dot{q}}\dot{f}dt.
$$

Look at the term with $\dot{f}$.  If we do integration by parts we get

$$
\int_{t_1}^{t_2}\frac{\partial\mathcal{L}}{\partial \dot{q}}\dot{f}dt = [\frac{\partial\mathcal{L}}{\partial \dot{q}}f]_{t_1}^{t_2} - \int_{t_1}^{t_2}f\frac{\text{d}}{\text{d}t}\frac{\partial\mathcal{L}}{\partial \dot{q}}dt,
$$

the term in the brackets is zero because function $f$ is defined to be zero at $t_1$ and $t_2$. Therefore we get the equation

$$
\frac{\text{d}S}{\text{d}\alpha}|_{\alpha = 0}=\int_{t_1}^{t_2}[\frac{\partial\mathcal{L}}{\partial q}-\frac{\text{d}}{\text{d}t}\frac{\partial\mathcal{L}}{\partial \dot{q}}]fdt  = 0
$$

since the variation along the minimum is equal to zero. So the generalized coordinates that give minimum action satisfy :

$$
\frac{\partial\mathcal{L}}{\partial q}-\frac{\text{d}}{\text{d}t}\frac{\partial\mathcal{L}}{\partial \dot{q}} = 0.
$$

This equation is called the Euler-Lagrange equation. Also known as the equations of motion.

#### Euler-Lagrange equations for system with multiple particles
Suppose we have system with $n$ particles. Then each particle in the system satifies
$$
\frac{\partial\mathcal{L}}{\partial q_i}-\frac{\text{d}}{\text{d}t}\frac{\partial\mathcal{L}}{\partial \dot{q}_i} = 0. \text{ For } 1\leq i \leq n. 
$$

To prove this do the same procedure as in derivation section on the following action

$$
S = \int_{t_1}^{t_2} \mathcal{L}(q_1,....q_n,\dot{q}_1,.....,\dot{q}_n)dt.
$$

##### Thoughts on EL-equations for multiple particles

I wonder if it is this property that leads to the additivity of Lagrangians. 

