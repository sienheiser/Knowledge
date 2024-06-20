---
aliases: [solid angles]
---

#math 


### Measuring a normal angle

Suppose we have a circle of radius $r$. If we were to take a slice from the circle with an angle of $\theta$, then the perimeter (arc length) would be given be 

$$
l = r\theta.
$$

We could rewrite the above expression as 

$$
\theta = \frac{l}{r}.
$$
This means that if we knew the arc lenght and radius of a slice we could define the angle. 

### Measuring a solid angle
A solid angle has a similar concept to an angle. Suppose we have a sphere with radius $r$. Suppose we take a cone out of that sphere. Using calculus, we could compute the surface area of the cone (only the top part) as 
$$
A = r^2\int_0^{2\pi} d\phi\int_0^{\frac{\theta}{2}}\sin(\theta)d\theta = 2\pi r^2 (1-\cos(\frac{\theta}{2}))
$$
where $\theta$ is the only from the $z-axis$ to the cone. We could rewrite the above expression as
$$
 2\pi(1-\cos(\frac{\theta}{2})) = \frac{A}{r^2}.
$$
The solid angle in this case is $\Omega =2\pi(1-\cos(\frac{\theta}{2}))$. So for a full sphere the solid angle it makes is $4\pi$. We can say that the solid angle is *the surface area of cone taken from a unit sphere*. An inifitesimal solid angle is written as 

$$
d\Omega = 2\pi \sin(\theta)d\theta.
$$
