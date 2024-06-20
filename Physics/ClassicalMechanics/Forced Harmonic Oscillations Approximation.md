#ClassicalMechanics 
### Approximating the External Potential
In [[Harmonic Approximation 1D|harmonic approximation 1D]] we learnt how to analyse a general system with stable equilibrium at $x = 0$. Suppose this system is exposed to an external field $U(x,t)_e$. For the small oscillation approximation to hold we have assume $U(x,t)_e$ is a weak field. We obtain the following Lagrangian:
$$
\mathcal{L} = \frac{m}{2}\dot{x}^2-\frac{k}{2}x^2-U(x,t)_e. \tag{1}
$$
If we taylor expand the external potential around $x = 0$ we get

$$
U(x,t)_e = U(0,t) + x \frac{\partial U}{\partial x}|_{x = 0} + .. \tag{2}
$$

The first term in the expansion purely depends on time meaning it is a total time derivative of another function which does not affect the equations of motions. The second term is the force times displacement which is the work done. We may consider higher order terms, but to simplify the equations we only take the first order term giving
$$
\mathcal{L} = \frac{m}{2}\dot{x}^2-\frac{k}{2}x^2-xF(t). \tag{3}
$$
### Equations of Motions with External Potential
We get the following equations of motion

$$
m\ddot{x} =kx-F(t) \iff \ddot{x} = -\omega^2 x-\frac{F(t)}{m}. \tag{4}
$$


