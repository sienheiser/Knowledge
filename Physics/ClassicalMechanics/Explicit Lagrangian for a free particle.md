---
aliases: [Free particle Lagrangian,Free particle, free particle Lagrangian in different coordinate systems]
---
#ClassicalMechanics
We discussed certain properties that the Lagranigan of a free particle must have in [[Galileo's Relativity Principle|properties of Lagrangian of free particle]] due to space being homogenous and isotropic. Here we will derive what the Lagrangian of a free particle must look like.

### Derivation of Lagrangian of free particle

Suppose we have two coordinate frames $K$ and $K^{'}$ where frame $K^{'}$ moves to the right of $K$ at a very small velocity $\vec{\epsilon}$. Suppose the free particle has constant velocity $\vec{v}$. Then the Lagrangian in frame $K$ looks like $\mathcal{L}(v^2)$ and the Lagnrangian in $K^{'}$ looks like $\mathcal{L}(v^{'2})=\mathcal{L}((\vec{v}-\vec{\epsilon})^2)$. Lets Taylor expand the at $\vec{\epsilon} = 0$ Lagrangian from  $K^{'}$, we get

$$
\mathcal{L}((\vec{v}-\vec{\epsilon})^2) = \mathcal{L}(v^2) - \vec{\epsilon}\cdot \frac{\partial \mathcal{L}(\vec{v}-\vec{\epsilon})^2}{\partial (\vec{v}-\vec{\epsilon})^2}\cdot \frac{\partial (\vec{v}-\vec{\epsilon})^2}{\partial \vec{\epsilon}}|_{\vec{\epsilon}=\vec{0}}= \mathcal{L}(v^2) - 2\vec{\epsilon}\cdot\vec{v}\frac{\partial \mathcal{L}(v^2)}{\partial v^2}.
$$

Since $\vec{\epsilon}$ is an infinitesimal velocity we do not consider terms above 1st order.  We know from [[Properties of Lagrangian|properties of Lagrangian]] that the equations of motion are not affected if a total time derivative of a function is added to a Lagrangian.  The only way 1st order term in the Taylor expansion can be a total time derivative of a function is if it is linear in velocity of the particle. As a result

$$
\mathcal{L}((\vec{v}-\vec{\epsilon})^2) =\mathcal{L}(v^2) - 2\vec{\epsilon}\cdot\vec{v}\frac{\partial \mathcal{L}(v^2)}{\partial v^2} = \mathcal{L}(v^2) - 2\frac{d}{dt}(\vec{\epsilon}\cdot\vec{r}\frac{\partial \mathcal{L}(v^2)}{\partial v^2}).
$$
Which implies that

$$
\frac{\partial \mathcal{L}}{\partial v^2} = constant \implies \mathcal{L} = \frac{1}{2}mv^2,
$$
where $m$ is the mass of the particle. 

### Frame moving with velocity $\vec{V}$

Suppose now that the $K^{'}$ is moving with velocity $\vec{V}$. Then the Lagrangian will look like
$$
\mathcal{L}(v^{'2}) = \mathcal{L}((\vec{v}-\vec{V})^2)) = \frac{1}{2}m(\vec{v}-\vec{V})^2 = \frac{1}{2}mv^2 -m \vec{v}\cdot\vec{V}-\frac{1}{2}mV^2.
$$
The $V^2$ term is just the velocity of the moving frame and is a constant. It does not affect equation of motion. The $m\vec{v}\cdot\vec{V}$ term can be rewritten as a total time derivative since $\vec{v} = \dot{\vec{x}}$.

### Free particle Lagrangian in different coordinate system
We know that $v^2 = (\frac{dl}{dt})^2 = \frac{dl^2}{dt^2}$ where $dl$ is a [[line element]]. In cartesian coordinates the [[line element]] is $dl^2 = dx^2+dy^2+dz^2$ which gives 
$$
\mathcal{L} = \frac{1}{2}m(\dot{x}^2+\dot{y}^2+\dot{z}^2).
$$
In cylindrical coordinates the line element is  $dl^2 = dr^2+r^2d\phi^2+dz^2$ which gives

$$
\mathcal{L} = \frac{1}{2}m(\dot{r}^2+r^2\dot{\phi}^2+\dot{z}^2).
$$

In spherical coordiantes the line element is  $dl^2 = dr^2+r^2d\theta^2+r^2\sin(\theta)d\phi^2$ which gives 
$$
\mathcal{L} = \frac{1}{2}m(\dot{r}^2+r^2\dot{\theta}^2+r^2\sin^2(\theta)\dot{\phi}^2).
$$



