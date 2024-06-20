---
aliases: [Properties of Lagrangian, properties of Lagrangian]
---
#ClassicalMechanics
### Properties of Lagrangian
If we look at [[Euler-Lagrange Equations|EL-equations]] for free particles we notice that each particle satisfies the an EL-equation. This suggests that for $n$ particle system we can writie the Lagrangian as
$$
\mathcal{L}(q_1,...,q_n,\dot{q}_1,.....,\dot{q}_n)=\sum_{i=1}^{n}\mathcal{L}_i(q_i,\dot{q}_i).
$$
Notice that the total $\mathcal{L}$ is the sum of the individual particles $\mathcal{L}_i$. 

Furthermore, ***multiplying a constant*** to $\mathcal{L}$ does not change the [[Euler-Lagrange Equations|equations of motion]]. Note that if there are multiple $\mathcal{L}_i$ being added. Then they all must be scaled by the same constant.

Suppose we add a total time derivative of an arbitrary function to the Lagrangian

$$
\mathcal{L}^`(q,\dot{q}) = \mathcal{L}(q,\dot{q})+\frac{\text{d}f(q,\dot{q})}{\text{d}t}.
$$
Then the equations of motion still remain the same. This can be seen from the [[Principle of Least Action|action]]
$$
S^` = \int^{t_2}_{t_1}\mathcal{L}^`(q,\dot{q})dt = \int^{t_2}_{t_1}\mathcal{L}(q,\dot{q})dt + f(q(t_2),\dot{q}(t_2)) - f(q(t_1),\dot{q}(t_1)) = S+ f(q(t_2),\dot{q}(t_2)) - f(q(t_1),\dot{q}(t_1)).
$$

If we were to use the variational principle what we see is the constants on the right disappear and do not affect the action.
#### Thoughts

In Landau's book, he says that the scalability is linked to the arbitrariness of units. 

It is interesting at face value that the two different actions still contain the same information. It seems that adding total time derivative function to the $\mathcal{L}$ is the same as just shifting the value the action.