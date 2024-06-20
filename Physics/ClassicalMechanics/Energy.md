---
aliases: [Energy, energy]
---
#ClassicalMechanics 

### energy
Since the Lagrangien is homogenous in time (see [[Galileo's Relativity Principle]] 1st paragraph). This means that the Lagrangian of a [[closed system]] does not depend on time explicitly. As a result the following is true
$$
\frac{d\mathcal{L}}{dt} = \sum_{i=1}^{n}\frac{\partial \mathcal{L}}{\partial q_i}\dot{q}_i + \frac{\partial \mathcal{L}}{\partial \dot{q_i}}\ddot{q}_i.
$$
Using [[Euler-Lagrange Equations|EL-equations]] we know $\frac{d}{dt}\frac{\partial \mathcal{L}}{\partial \dot{q}} = \frac{\partial\mathcal{L}}{\partial q}$ which give

$$
\frac{d\mathcal{L}}{dt} = \sum_{i=1}^{n}\frac{d}{dt}\frac{\partial \mathcal{L}}{\partial \dot{q}_i}\dot{q}_i + \frac{\partial \mathcal{L}}{\partial \dot{q_i}}\ddot{q}_i = \frac{d}{dt}\sum_{i=1}^{n}\frac{\partial \mathcal{L}}{\partial \dot{q}_i}\dot{q}_i \implies \frac{d}{dt}(\sum_{i=1}^{n}\frac{\partial \mathcal{L}}{\partial \dot{q}_i}\dot{q}_i-\mathcal{L}) = 0.
$$

We define the energy of the system to be 

$$
E = \sum_{i=1}^{n}\frac{\partial \mathcal{L}}{\partial \dot{q}_i}\dot{q}_i-\mathcal{L}.
$$
To see why this is the case. We know that $\sum_{i=1}^{n}\frac{\partial \mathcal{L}}{\partial \dot{q}_i}\dot{q}_i$ is a [[homogenous function]] that is quadratic  in $\dot{q}_i$. Meaning $\sum_{i=1}^{n}\frac{\partial \mathcal{L}}{\partial \dot{q}_i}\dot{q}_i =2T$. Therefore, $E = 2T-(T-E) = T+E$ which is the total energy of the system.
