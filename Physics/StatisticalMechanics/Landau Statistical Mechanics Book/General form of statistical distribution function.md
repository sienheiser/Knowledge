---
aliases: []
---
#StatisticalMechanics 

The statistical distribution function can be seen as a [[Integrals of the motion]]. This is explained in [[Statistical distribution function as a integral of the motion|statistical distribution function as a integral of the motion]]. If we look at a composite system of two subsystems then their statistical disrtibution function has the following property (due to [[Statistical Independence]])
$$
\mathcal{Q}_{12} = \mathcal{Q}_{1}\mathcal{Q}_{2} \implies \log(\mathcal{Q}_{12}) = \log(\mathcal{Q}_{1})+\log(\mathcal{Q}_{2}).
$$
This means that the logarithm of of distribution function must be additive integrals of the motion. To elaborate, we want integrals of the motion that are defined for seperate systems, but can be added together to make a whole system. The only ones that satisfy this condition are [[Energy|energy]],[[Momentum (Classical mechanics)|momentum]] and [[Angular momentum (Classical Mechanics)|angular momentum]] of the subsystem. This means that there 7 conserved quantites (energy, three components of momentum and three components of angular momentum). Let $E_a(p,q)$, $\vec{P}_a(p,q)$ and $\vec{M}_a(p,q)$ be the energy, momentum and angular momentum of the $a$th system. These quantities depend on positions $q$ and momentum $p$ of the particles within the $a$th subsystem. The only additive form of $\log\mathcal{Q}_a$ is a linear combinations of energy, momentum and angular momentum 
$$
\log\mathcal{Q}_a = \alpha_a+\beta E_a(p,q)+\vec{\gamma}\cdot\vec{P}_a(p,q)+\vec{\delta}\cdot\vec{M}_a(p,q)
$$
with constant coefficients $\beta, \vec{\gamma}$ and $\vec{\delta}$ for the entire system and $\alpha_a$ also a constant but can be unique for each subsystem. The constant $\alpha_a$ is a normalization constant determined from $\int\mathcal{Q}_adp_adq_a = 1$. Not sure how the rest of the constants are determined.

We reach an important conclusion in statistical physics. **The values of the additive integrals of the motion completely define  the properties of a closed system **.