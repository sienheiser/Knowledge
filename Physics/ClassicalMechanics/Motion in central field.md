---
aliases: []
---
#ClassicalMechanics 

### Motion in central field

We know the form of the Lagrangian for two body system from [[Two-Body problem reduction]]. If placed in spherical coordinates 

$$
\mathcal{L} = \frac{1}{2}m(\dot{r}^2+r^2\sin^2(\theta)\dot{\phi}^2+r^2\dot{\theta}^2)-U(r).
$$

If we set $\theta=\frac{\pi}{2}$ then $\sin(\theta) = 1$ and $\dot{\theta} = 0$. This means allow the particle orbit the course in the xy-plane. We see that the $\phi$ is a cyclic coordinate meaning it is conserved. As a result in this case the angular momentum along z-axis is conserved. This $M = mr^2\dot{\phi}$ is conserved. The Lagrangian can be rewritten as

$$
\mathcal{L} = \frac{1}{2}m\dot{r}^2+\frac{M^2}{2mr^2}-U(r).
$$
Then by using the conservation of energy we get 

$$
t = \int \frac{dr}{\sqrt{\frac{2}{m}(E-U_{\text{eff}}(r))}}
$$
where $U_{\text{eff}}(r) = U(r)+\frac{M^2}{2mr^2}$. Furthermore, using the relation $M = mr^2\dot{\phi}$ and conservation of energy we get

$$
\phi = \int \frac{Mdr/r^2}{\sqrt{2m(E-U_{\text{eff}}(r))}}.
$$

Given that we know the maximum distance and minimum distance between the source and the oribiting particle. We can calculate the time it takes for the particle to reach from $r_{min}$ to $r_{max}$, similarly we can calculate the angle between $r_{min}$ to $r_{max}$. 

