#ClassicalMechanics 

In [[Disintegration of two particle (lab frame)]] we found relation between the the velocity of particle in lab frame and center of mass frame. This is an interesting way of visualizing the two velocities.

![[CoolVisualizationVelocities.jpg]]
In the above figure two circles with radius $|\vec{v}_0|$ are drawn. $\vec{v}_0$ is the velocity of the particle in the center of mass frame, $\vec{V}$ is the of the center of mass frame w.r.t the lab frame and $\vec{v}$ is the velocity of the particle in the lab frame. The angle $\theta$ is the angle between vectors $\vec{V}$ and $\vec{v}$; the angle $\theta_0$ is the angle between vectors $\vec{V}$ and $\vec{v}_0$. Note that angle $\theta$ should be drawns on the right circle also. These circles represent two cases: if $V<v_0$ on the left and if $V>v_0$ on the right. Notice that if we rotate $v_0$ the angle $\theta$ on the left has possible values $[0,2\pi]$. On the right side this is not the case. There is a maximum angle $\theta$ can take and it satifies

$$
\sin\theta_{\text{max}} = \frac{v_0}{V}.
$$

To find the relation between angles $\theta$ and $\theta_0$ we imagine drawing a line starting from where vectors $\vec{v}$ and $\vec{v}_0$ straight down to the dashed horizontal line. Then we have formed a right angle triangle. We get the following relation
$$
\tan\theta = \frac{v_0\sin\theta_0}{V+v_0\cos\theta_0}
$$
which has solutions

$$
\cos\theta_0 = -\frac{V}{v_0}\sin^2\theta \pm \cos\theta \sqrt{1-\frac{V^2}{v_0^2}\sin^2\theta}
$$