---
aliases: [classical mechanics problems]
---
#ClassicalMechanics 
### Problem Chapter 1 Landau 
Find the Lagrangian of each of the following systems when placed in a uniform gravitational field.

##### Problem 1: Coplanar Double Pendulum
Using the spherical coordinates from [[Explicit Lagrangian for a free particle|free particle Lagrangian in different coordinate systems]] we see that that mass $m_1$ has only one degree of freedom so its line element is $dl^2 = l_1^2\phi_1^2$. The potential of the system is only dependent on the heignt at which mass $m_1$ is at. So, $U = -m_1gl_1\cos(\phi_1)$. To explain the minus sign we can set $l_1\cos(\phi_1) = y_1$. Then we see that as $y_1$ increases the potential decreases and as $y_1$ decreases the potential increases. Therefore, as $-y_1$ increases the potential also increases. So we add the minus sign to align the potentials and $y_1$ behaviour. As a result the Lagrangian of the first mass is 
$$
\mathcal{L}_1 = \frac{1}{2}m_1l_1^2\dot{\phi_1^2} + m_1gl_1\cos(\phi_1).
$$
The next mass has degree of freedom 2. Meaning it can reach anywhere on the plane. This means we need to describe its position using two coordinates. Let $(x_1,y_1)$ be position coordinates of (they are also generalized coordinates) mass $m_1$. Let $(x_2,y_2)$ be position coordinates of mass $m_2$. Then we see that 
$$
x_2 = x_1 + l_2\sin(\phi_2) = l_1\sin(\phi_1)+l_2\sin(\phi_2). 
$$

To check if this is correct look if $\phi_1=\phi_2 = 0$ we expect $x_2 = 0$ which is case with how we have defined the coordinates above. Similarly $\phi_1=\phi_2 = \pi/2$ then $x_2 = l_1+l_2$ which is also the case with the above coordinates. Using similar arguements we get
$$
y_2 = l_1\cos(\phi_1)+l_2\cos(\phi_2).
$$
The Lagrangian for the second mass is

$$
\mathcal{L}_2 = \frac{1}{2}m_2((l_1\dot{\phi_1}\cos(\phi_1)+l_2\dot{\phi_2}\cos(\phi_2))^2 + (-l_1\dot{\phi_1}\sin(\phi_1)-l_2\dot{\phi_2}\sin(\phi_2))^2) + m_2g(l_1\cos(\phi_1)+l_2\cos(\phi_2)).
$$
After using trig identities and simplifying the expression we get that 

$\mathcal{L}_2 = \frac{1}{2}m_2(l_1^2\dot{\phi_1}^2+l_2^2\dot{\phi_2}^2+2l_1l_2\dot{\phi_1}\dot{\phi_2}\cos(\phi_1-\phi_2))+m_2g(l_1\cos(\phi_1)+l_2\cos(\phi_2))$.


So the final Lagrangian is 

$$
\mathcal{L} = \mathcal{L}_1 + \mathcal{L}_2 =  \frac{1}{2}m_1l_1^2\dot{\phi_1^2} +\frac{1}{2}m_2(l_1^2\dot{\phi_1}^2+l_2^2\dot{\phi_2}^2+2l_1l_2\dot{\phi_1}\dot{\phi_2}\cos(\phi_1-\phi_2))+m_1gl_1\cos(\phi_1)+m_2g(l_1\cos(\phi_1)+l_2\cos(\phi_2))
$$

##### Comments on solving rest of the problems in Landau Classical mehcanics chapter 1

It seem like the best thing to do it draw a Cartisian coordinate system first. Then write out the Lagrangians in the Cartesian coordinate systems. If the problem 
has polar coordiantes sysmmetry then convert the cartesian coordinates to the polar coordinates. So far with all the problems this scheme has not failed. 

Try looking at the [[Degrees of Freedom|degrees of Freedom]] of a system. This immediately gives information on how many generalized coordinates are needed.



### Problem in unit 7 Landau
A particle of mass $m$ moving with velocity $\vec{v_1}$ leaves a half-space where the potential is a constant $U_1$ and enters another in which the potential is a different constant $U_2$. What is the change in direction of the motion of the particle?
![[HalfSpaceAndPotential.jpg]]
Suppose we split space into two halves as in the right side coordiate system in the above figure. Then the potential is along the $y$-direction. The potential is plotted in the left plot. A particle coming from $y=-\infty$ to $y =\infty$ will experience an acceleration at $y = 0$. According to the conservation of energy, the energy of the particle in the first half is equal to the energy of the particle in the second half i.e.

$$
\frac{1}{2}mv_1^2+U_1 = \frac{1}{2}mv_2^2+U_2.
$$
This implies that 
$$
v_2 = \sqrt{v_1^2-2\frac{U_1-U_2}{m}}.
$$

Now we know that the particle accelerates along the y-axis after entering the second half of the space. This means that momentum is only conserved along the xz-plane. If we define $\theta_1$ to be the angle between the y-axis and the particles velocity $\vec{v}_1$ then the projection of the particle's velocity onto the xz-plane is $v_1\sin \theta_1$. Similarly after the particle has entered the second half of space its projected velocity onto the xz-plane is $v_2\sin \theta_2$. Due to conservation of momentum along the xz-plane we have
$$
\frac{\sin\theta_1}{\sin\theta2} = \frac{v_2}{v_1} = \sqrt{1-2\frac{U_1-U_2}{mv_1^2}}.
$$
From this we can find $\theta_2$. 



### Problem in unit 8 Landau

Find the law of transformation of the action $S$ from one inertial frame to another inertial frame.

We know from [[Center of Mass (classical mechanics)#energy between two frames]] that energy transforms as

$$
E = E^{'}+\vec{P}^{'}\cdot\vec{V}+\mu V^2.
$$
between two inertial frames. Similarly the Lagrangian of a system should also also obey the same law (***prove this***)

$$
\mathcal{L} = \mathcal{L}^{'}+\vec{P}^{'}\cdot\vec{V}+\mu V^2.
$$

Then the action becomes

$$
S = \int \mathcal{L} dt = \int \mathcal{L}^{'}+\vec{P}^{'}\cdot\vec{V}+\mu V^2 dt = S^{'}+\vec{R}^{'}\cdot\vec{V}+\mu V^2t
$$
where $\vec{R}^{'}$ is the center of mass vector in the other frame.


### Problem 3 in unit 9 Landau
Which compoenets of momentum $\vec{P}$ and angluar momentum $\vec{M}$ are conserved in motion in the following fields?
(a) the field of an infinite homogenoun plane, (b) that of an infinite homogenous cylinder,(c) that of an infite homogenous prism,(d) that of two points, (e) that of an infinite homogenous half-plane, (f) that of a homoganous cone, (g) that of a homogenous circular torus, (h) that of an infinte homogenous cylindrical helix.

![[SymmetricalFields.jpg]]
Imagine in each case we have the Lagrangian $L$ of the system. What we can do is then test the Lagrangian for symmetries of the system. Scheme for testing the the symmetries of the system. Place a test particle near the field source then only translate and rotate the field source while leaving the test particle in the same position.

(a) If we translate the infinite place in the x or y direction the test particle still sees the same field. If we rotate the plane about the z-axis the test particle still sees the same field. Therefore, $p_x$, $p_y$ and $M_z$ are conserved.

(b) The infinite cylinder is symmetric w.r.t translation along z-axis and rotations about z-axis. So $p_z$ and $M_z$ are conserved.

(c) not sure what a prism is?

(d) Only symmetry for two points is rotation about the z-axis. So $M_z$ is conserved.

(e) Only symmetry for infinite half plane is tranlsation along the y-axis. So $p_y$ is conserved.

(f) Only symmetry for homogenous cone is rotation about the z-axis. So $M_z$ is conserved. 

(g) Only symmetry for circular torus is rotation about the z-axis. So $M_z$ is conserved.

(h) Symmerty of cylindrical helix not immediately obvious. However if translate the cylinder by distance $h$ along z-axis and rotate the cylinder by $2\pi$ about z-axis. Then the cylindrical helix is symmetric. This means that 

$$
\mathcal{L}(r,\phi+\delta\phi,z+\delta z) = \mathcal{L}(r,\phi,z)+\delta\phi\frac{\partial\mathcal{L}(r,\phi,z)}{\partial \phi}+\delta z\frac{\partial\mathcal{L}(r,\phi,z)}{\partial z}
$$

which implies 

$$
\delta \mathcal{L} = \delta\phi\frac{\partial\mathcal{L}(r,\phi,z)}{\partial \phi}+\delta z\frac{\partial\mathcal{L}(r,\phi,z)}{\partial z} = 2\pi\dot{M}_z+h\dot{p}_z\implies 2\pi M_z+h p_z=\text{constant}.
$$
Notice how the for the other cases we had the freedom to translate or rotate any amount to get sysmetries. In this case we can only translate a specific amount and rotate a specific amount. 


### Problem 1 unit 11 Landau

Determine the period of oscillations  of a simple pendulum as a function of the amplitude and the oscillations.

We know that 
$$
\mathcal{L} = \frac{m}{2}l^2\dot{\phi}^2+mgl\cos(\phi).
$$

If $\phi_0$ is the max angle that the pendulmn can reach then the total energy of the system is $E = -mgl\cos(\phi_0)$. There is a minus sign because our potential $U = -mgl\cos(\phi)$. Therefore the total energy can be written as 
$$
E = \frac{m}{2}l^2\dot{\phi}^2-mgl\cos(\phi) = -mgl\cos(\phi_0).
$$
If it takes time $t$ to go from $\phi=0$ to $\phi=\phi_0$. Then the period of the pendulum is $T = 4t$. This means that 

$$
T = 4\sqrt{\frac{m}{2}}\int_{0}^{y_0}\frac{dy}{\sqrt{E+mgy}} = 4\sqrt{\frac{m}{2}}\int_{0}^{\phi_0}\frac{ld\phi}{\sqrt{-mgl\cos(\phi_0)+mgl\cos(\phi)}}.
$$

After some rewriting we get

$$
T = 4\sqrt{\frac{l}{2g}}\int_{0}^{\phi_0}\frac{d\phi}{\sqrt{-\cos(\phi_0)+\cos(\phi)}}.
$$
If we use identity $\cos(\phi) = 1-2\sin^2(\frac{\phi}{2})$ then 

$$
T = 2\sqrt{\frac{l}{g}}\int_{0}^{\phi_0}\frac{d\phi}{\sqrt{\sin^2(\frac{\phi_0}{2})-\sin^2(\frac{\phi}{2})}}.
$$
Setting $\sin(\eta) = \frac{\sin(\frac{\phi}{2})}{\sin(\frac{\phi_0}{2})}$ gives $T = 4\sqrt()$


### Problem 1 unit 13 Landau

A system contains one particle of mass $M$ and $n$ particles of mass $m$. Eliminate the motion of the center of mass  and so reduce the problem to one involving $n$ particles.


We may imagine radius vector $\vec{R}$ points arbitrary origin to particle with mass $M$. We may also imagine raidus vectors $\vec{R}_a$ pointing from the same arbitrary origin to particles with mass $m_a$. 
To eliminate the the motion of the center of mass we should compute the radius vector that points from the arbitrary origin to the center of mass, and set it so that the center of mass radius vector points towards the origin. The center of mass vector can be computed using the scheme in [[Center of Mass (classical mechanics)|center of mass]]. This gives 

$$
\vec{R}_{\text{COM}} = \frac{M\vec{R}+m\sum_{i=1}^n\vec{R}_i}{M+nm}=0,
$$
where $\vec{R}_{\text{COM}}$ is equal to zero because we want it to point at the origin. Then we may define vectors $\vec{r}_a = \vec{R}_a-\vec{R}$ which point from particle with mass $M$ to particles with mass $m$. If we substitute $\vec{r}_a+\vec{R} = \vec{R}_a$ in the center of mass relation we get 
$$
M\vec{R}+m\sum_{i=1}^n(\vec{r}_i+\vec{R}) = 0 \implies \vec{R} = -m\frac{\sum_{i=1}^n\vec{r}_i}{M+nm}.
$$

The original Lagrangian is 
$$
\mathcal{L} =\frac{1}{2}M\dot{R}^2+\frac{1}{2}m\sum_{i=1}^n\dot{R}^2_i-U.
$$
subbing in the new experession in terms of vectors $\vec{r}_i$ gives 

$$
\mathcal{L} =\frac{1}{2}M\left(-m\frac{\sum_{i=1}^n\dot{\vec{r}}_i}{M+nm}\right)^2+\frac{1}{2}m\sum_{i=1}^n\left(\dot{\vec{r}}_i+\dot{\vec{R}}\right)^2-U.
$$

Expanding the second sum gives $\left(\dot{\vec{r}}_i+\dot{\vec{R}}\right)^2 = \frac{m}{2}\sum v_i^2+\vec{R}\cdot m\vec{P}+\dot{R}^2$. The momentum $\vec{P}$ is zero since we are in center of mass coordinates. The term $\dot{R}^2 =(m\frac{\sum_{i=1}^n\dot{\vec{r}}_i}{M+nm})^2$ giving Lagrangian 

$$
\mathcal{L} = \frac{m^2}{2(M+nm)}\left(-m\frac{\sum_{i=1}^n\dot{\vec{r}}_i}{M+nm}\right)^2+\frac{1}{2}m\sum_{i=1}^n\left(\dot{\vec{r}}_i\right)^2-U.
$$
***Note that the first term on the RHS has a minus in Landau's book. But I do not see where it comes from.***

