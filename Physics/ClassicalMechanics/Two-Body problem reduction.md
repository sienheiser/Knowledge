---
aliases: []
---

#ClassicalMechanics 


Suppose we have two masses and the potential only depends between the distances of their center of mass. Let $\vec{r}_1$ and $\vec{r}_2$ point to masses $m_1$ and $m_2$ repectively. Then the Lagrangian might look like 
$$
\mathcal{L} = \frac{1}{2}(m_1\dot{r}_1^2+m_2\dot{r}_2^2)-U(|\vec{r}_1-\vec{r}_2|).
$$

Let us define another frame $K^{'}$ moving w.r.t to the original frame. Then by using the scheme from [[Center of Mass (classical mechanics)|center of mass]] we may define a center of mass frame. Suppose the prime frame moves with velocity $\vec{V}$ then $\vec{r} = \vec{r}^{'}+\vec{V}t$. So the total momentum is $\vec{P} = \sum_a m_av_a=\sum_a m_a(v_a^{'}+\vec{V}) = \vec{P}^{'}+\vec{V}\mu$. Want $\vec{P}^{'} = 0\implies \vec{V} = \frac{\vec{P}}{\mu}$. Now using this equaition we can derive the radius vector pointing to the center of mass of the system by $\frac{\vec{P}}{\mu} = \frac{\sum_a m_a\vec{\frac{d\vec{r}_a}{dt}}}{\sum_a m_a}=\frac{d\vec{R}}{dt}\implies \vec{R} = \frac{\sum_a m_a r_a}{\sum_a m_a}$. In our case we have two masses so vector
$$
\vec{R} = \frac{m_1\vec{r}_1+m_2\vec{r}_2}{m_1+m_2}
$$
points to the center of mass of the system. We can set $\vec{R}=0$ means it points to the origin (so our origin is the center of mass) and can define speration vector $\vec{r} = \vec{r}_1-\vec{r}_2$. This gives use 

$$
\vec{r}_1 = m_2\frac{\vec{r}}{m_1+m_2},\quad \vec{r}_2 = -m_1\frac{\vec{r}}{m_1+m_2}
$$
which gives 
$$
\mathcal{L} = \frac{m}{2}\dot{\vec{r}}-U(r),
$$
where $m = \frac{m_1m_2}{m_1+m_2}$ is the reduced mass.

Landau's says that the interaction of two particles is equivalent to the motion of a particle in field $U(r)$.

