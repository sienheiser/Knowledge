---
aliases: [Louville's theorem]
---
### Louville's theorem statistical mechanics
From [[Phase Points as Gas|phase points as gas]] we know we take a statitical ensemble of phase spaces of a subsystem overlap them and allow the [[Phase Space|phase space]] to evolve. The end result is, the phase radius vectors behave as 'gas' particles. The flow of these 'gas' particles obeys the [[continuity equation|continuity equation]]
$$
\frac{\partial \mathcal{Q}}{\partial t}+\nabla\cdot(\vec{v}\mathcal{Q}) = 0
$$
where $\mathcal{Q}$ is the [[Statistical distribution in statical mechanics|statistical distribution]] function for the subsystem and $\vec{v}$ is the velocity of the 'gas'.

Since our statistical distribution does not change in time (see [[Finding the statistical distribution|finding statisitcal distribution]]) $\frac{\partial \mathcal{Q}}{\partial t} = 0$. This leaves as with 

$$
\nabla\cdot(\vec{v}\mathcal{Q}) = \sum_{i=1}^{2s} \frac{\partial(\mathcal{Q}v_i)}{\partial x_i} = 0,
$$
where $x_i$ represents both the [[Generalized Coordiantes|generalized coordinates]] $q_i$ and the generalized momenta $p_i$ (see [[Momentum (Classical mechanics)#generalized momenta and generalized forces]]). We can rewrite the $v_i = \dot{x}_i$. This gives 

$$
\sum_{i = 1}^s\left[ \frac{\partial(\mathcal{Q}\dot{q}_i)}{\partial q_i}+\frac{\partial(\mathcal{Q}\dot{p}_i)}{\partial p_i}\right] = 0.
$$
Expanding the derivatives give 
$$
\sum_{i = 1}^s \left [\dot{q}_i\frac{\partial(\mathcal{Q})}{\partial q_i} + \dot{p}_i\frac{\partial(\mathcal{Q})}{\partial p_i} \right] + \mathcal{Q}\sum_{i = 1}^s \left [\frac{\partial(\dot{q}_i)}{\partial q_i} + \frac{\partial(\dot{p}_i)}{\partial p_i} \right] = 0.
$$
The second bracket is equal to zero due to [[Hamilton's equations of motion]]

$$
\dot{q}_i = \frac{\partial \mathcal{H}}{\partial p_i}, \dot{p}_i = -\frac{\partial \mathcal{H}}{\partial q_i}, 
$$

These equations of motion imply $\frac{\partial\dot{q}_i}{\partial q_i} =\frac{\partial^2\mathcal{H}}{\partial q_i\partial p_i} = -\frac{\partial\dot{p}_i}{\partial p_i}$. So we finally get

$$
\frac{d\mathcal{Q}}{dt}=\sum_{i = 1}^s \left [\dot{q}_i\frac{\partial(\mathcal{Q})}{\partial q_i} + \dot{p}_i\frac{\partial(\mathcal{Q})}{\partial p_i} \right] = 0.
$$
The right hand side is just the total time derivative of the statistical distribution function. The important conclusion we come to is that the distribution function does not change along phase trajectories of a subsystem. This is ***Louville's theorem***. The result is only valid when considering the [[quasi-closed system|quasi-closed system]] under small time intervals which essentially makes them closed systems.

