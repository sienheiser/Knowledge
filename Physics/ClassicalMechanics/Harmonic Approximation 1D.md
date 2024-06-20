#ClassicalMechanics 

### One Dimension Harmonic Approximation
Suppose we consider a system with one [[Degrees of Freedom|degree of freedom]]. The general Lagrangian is written as 

$$
\mathcal{L} = \frac{1}{2}a(q)\dot{q}^2 - U(q) \tag{1}
$$
where $U(q)$ is the potential of the system. Suppose that the system has a stable equilibrimum at point $q_0$ (that is the minimum of potential). We can study the behaviour of the system when it is at and moves slightly away from $q_0$. The Taylor expansion of $U$ at point $q_0$ is
$$
U(q) = U(q_0) + (q-q_0)\frac{dU}{dq}|_{q = q_0} + \frac{(q-q_0)^2}{2}\frac{d^2 U}{dq^2}|_{q=q_0} + ... \tag{2}
$$

We are free set $U(q_0) = 0$ as the minimum of the potential and introduce $x = q-q_0$ which changes equation (2) to 
$$
U(x) = \frac{k}{2}x^2. \tag{3}
$$
We get the Lagrangian to be 

$$
\mathcal{L} = \frac{1}{2}a(x+q_0)\dot{x}-\frac{k}{2}x^2. \tag{4}
$$
Since the system is near the minimum most of the time we may set $a(x+q_0) = a(q_0) = m$. 
### Solutions to the Approximations

Then using the [[Euler-Lagrange Equations|EL-equations]] we get the following differential equation
$$
m\ddot{x} = -kx \iff \ddot{x} = \omega^2x \quad \text{where}\quad \omega = \sqrt{\frac{k}{m}} \tag{5}.
$$

The general solution to equaion (5) is $x = A\cos(\omega t)+B\sin(\omega t) = C\cos(\omega t+\alpha)$. Where $C$ and $\alpha$ are determinted by inital conditions.

Note that the quantity $\omega$ is completely determined by the mechanical properties of the system. This is as long as the oscillation of the system are small. With big oscillations the theory breaks down.

### The energy of the system in small oscillations
We have defined the [[Energy|energy]] as $E = p\dot{q} - \mathcal{L} = \frac{1}{2}m\dot{x}^2+\frac{k}{2}x^2= \frac{a^2\omega^2 m}{2}$. So the energy of the system for small oscillations only depends on the amplitude, intrinsic frequency $\omega$ and 'mass' $m$.

