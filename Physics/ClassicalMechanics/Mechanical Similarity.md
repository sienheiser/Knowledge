---
aliases: [mechanical similarity]
---
#ClassicalMechanics 


### mechanical similarity
Suppose potential is [[homogenous function|homogenous function]] of coordinates with property 
$$
U(\alpha \vec{r}_1,...,\alpha\vec{r}_n) = \alpha^kU( \vec{r}_1,...,\vec{r}_n).
$$
Suppose we scale all coordinates by $\alpha$ and time by $\beta$. Then the Lagrangian for a system of particles becomes

$$
\mathcal{L} = \frac{\alpha^2}{\beta^2}\frac{1}{2}\sum_a m_a v_a^2- \alpha^k U(\vec{r}_1,...,\vec{r}_n).
$$
For the Lagrangian to remain the same (see [[Properties of Lagrangian|properties of Lagrangian]])$\frac{\alpha^2}{\beta^2}= \alpha^k\implies\beta=\alpha^{1-\frac{1}{2}k}$. Suppose the length of the path for $\mathcal{L}(q,\dot{q})$ is $l$ and $\mathcal{L}(q',\dot{q}')$ is $l'$. Using line elements we can deduce the relation between $l$ and $l'$. The line element $dl = \sqrt{\sum_i (dq_i)^2}$ and the line element $dl' = \alpha\sqrt{\sum_i(dq_i)^2} =\alpha dl$ which means that $l'/l = \alpha$. The below relations can be found using the ratios between coorinates and scaled coordiantes. 

$$
\frac{t}{t^{'}} = \left(\frac{l}{l^{'}}\right)^{1-\frac{1}{2}k},\quad \frac{v}{v^{'}} = \left(\frac{l}{l^{'}}\right)^{\frac{1}{2}k},\quad \frac{E}{E^{'}} = \left(\frac{l}{l^{'}}\right)^{k}\quad \frac{M}{M^{'}} = \left(\frac{l}{l^{'}}\right)^{1+\frac{1}{2}k}.
$$

To see an explicit example see [[mechanical similarity problem]]. This is useful for finding proportinalities between the path and other quantities. For example, if we have a ball at height $h$ and drop it in a uniform gravitaional field. In this case $k=1$. Then we have $y = -gt^2+h$ the time it take for the ball to hit the ground is $t=\sqrt{\frac{h}{g}}$. Notice how time is directly proportional to altitude. Similarly for Newtonian attraction between two masses or Coloumb's law, the potential is homogenous function with $k = -1$ this means that $\frac{t}{t^{'}} =\left(\frac{l}{l^{'}}\right)^{\frac{3}{2}}$. As a result we can say that the time squared of a revolution is directly proportional to the cubed length of the orbit (Kepler's third law). 

