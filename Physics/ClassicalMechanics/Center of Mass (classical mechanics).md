---
aliases: [Center of mass, center of mass, COM]
---

#ClassicalMechanics 


### center of mass frame

The total momentum of a closed mechanical system is different in different inertial frames. Suppose we have two frames $K$ and $K^{'}$, where the latter moves with velcotiy $\vec{V}$ w.r.t $K$. Then using the [[Galileo's Relativity Principle#Galilean coordinate transformation between two frames]] which gives $\vec{r} = \vec{r}^{'}+\vec{V}t$. Then taking the total time derivative gives $\vec{v} = \vec{v}^{'}+\vec{V}$.  Then the total momentum is 
$$
\vec{P} = \sum_a m_a\vec{v}_a = \sum_a m_a\vec{v}_a^{'} + \vec{V}\sum_a m_a = \vec{P}^{'}+\vec{V}\sum_a m_a
$$
Now suppose we want a frame where $\vec{P}^{'} = \vec{0}$. Such a frame can always be chosen. Then we find that 
$$
\vec{V} = \frac{\sum_a m_a\vec{v}_a}{\sum_a m_a}.
$$
The above formula has interesting implications. Basically, if you have a closed system where you add all the momenta but you find that it is not zero. Then you can find another frame where the total momenta of is zero. Just make the other frame move at velocity $V$ w.r.t your initial frame. Notice how the above formula has the same form as momentum of a single particle $p = mv$ where $m$ in this case is the total mass of the system. 

### center of mass of the system
We have derived 
$$
\vec{V} = \frac{\sum_a m_a\vec{v}_a}{\sum_a m_a}.
$$
We can rewrite it as 
$$
\frac{d\vec{R}}{dt} = \frac{\sum_a m_a\frac{d\vec{r}_a}{dt}}{\sum_a m_a}\implies \vec{R} = \frac{\sum_a m_a\vec{r}_a}{\sum_a m_a}
$$

### law of conservation of momentum 
The law of conservaiton of momentum for a closed system can be reformulated as stating that the center of mass of a system moves in uniformly in a straight line. This also generalizes the law of interia derived for a free particle  (see [[Galileo's Relativity Principle#The form of Lagrangian of a free paritcle]]).

### energy between two frames
Suppose we have two frames $K$ and $K^{'}$, where the latter moves with velcotiy $\vec{V}$ w.r.t $K$. Then we know $\vec{v} = \vec{v}^{'}+\vec{V}$.  Therefore
$$
E = \sum_a \frac{1}{2}m_av_a^2 = \sum_a \frac{1}{2}m_a(\vec{v}^{'}_a+\vec{V})^2 =\sum_a \frac{1}{2}m_a (v^{'2}_a+2\vec{v}^{'}_a\cdot \vec{V}+V^2).
$$
The energy can be rewritten as

$$
E = E^{'}+\vec{P}^{'}\cdot\vec{V}+\mu V^2.
$$
If $K^{'}$ is the center of mass frame then $\vec{P}^{'} = 0$. This gives
$$
E = E^{'}+\mu V^2
$$
which is expected.
