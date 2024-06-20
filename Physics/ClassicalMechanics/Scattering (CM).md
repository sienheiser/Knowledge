---
aliases: [scattering]
---

#ClassicalMechanics 

In [[Motion in central field| motion in central field]] we derived the equation to find the angle $\phi$ if a particle changes its radius while in the presence of a central field

$$
\phi = \int \frac{Mdr/r^2}{\sqrt{2m(E-U(r))-\frac{M^2}{r^2}}}.
$$

![[Deflection.png]]

The figure above depicts a particle coming from the right towards the left from infinity. It gets deflected by angle $\chi$. From the image it is clear that $\chi = |\pi-2\phi_0|$. The term $\rho$ is known as the impact parameter. It is the distance at which the particle would pass the centre if the there was no field of force. We can rewrite the $E$ and $M$ in terms of the impact parameter $\rho$ and velocity of the particle at infinity $v_{\infty}$. So $E = 1/2 mv_{\infty}^2$ and $M = mv_{\infty}\rho$. This gives $\chi$ as a function of impact parameter. The larger the impact parameter the smaller $\chi$.

Usually we deal with the scattering of a beam of particles all with same velocity $\vec{v}_{\infty}$. Let $dN$ be the number of particles scattered between angle $\chi$ and $\chi +d\chi$ per unit time. This number is dependent on the density of the beam. If $n$ is the number of particles per unit area per unit time in the beam then 
$$
d\sigma = \frac{dN}{n}
$$
which has dimensions area. It is entirely determined by the form of scattering field. It is known as the scattering cross section. 

Assume that the relation between $\rho$ and $\chi$ is one to one (resonable assumption). Then only particles whose impact parameters lie between $\rho$ and $\rho +d\rho$ are scattered through angles $\chi$ and $\chi +d\chi$. This means the total number of particles being scattered between $\chi$ and $\chi +d\chi$ is the area of the circle between $\rho$ and $\rho +d\rho$ times the density of the beam i.e. $dN = 2\pi \rho n d\rho$. This means

$$
d\sigma = 2\pi\rho d\rho
$$

To get the relation between scattering cross section and $\chi$ we simply do

$$
d\sigma = 2\pi \rho |\frac{d\rho}{d\chi}|d\chi.
$$
We use the modulus since the derivative may be negative. To express this in terms of solid angles: Define $d\Omega$ as the solid angle between the cones with verticle angles $\chi$ and $\chi+d\chi$. This is given as $d\Omega = 2\pi \sin\chi d\chi$ which finally gives as the expression

$$
d\sigma = \frac{\rho(\chi)}{\sin(\chi)}|\frac{d\rho(\chi)}{d\chi}|d\Omega
$$

### Interpretation of scattering cross section
The scattering cross section can be interpreted as a sort of probability for a certain event to occur. Example suppose we have a simple hard sphere with radius $R$ fixed into position and we have an incidence beam. We may ask what is the scattering cross section for particles to be deflected between angles $\chi_0$ and $\chi_1$. This quantity does not depend on the density of incidence beam, only on the type of scattering potential present.