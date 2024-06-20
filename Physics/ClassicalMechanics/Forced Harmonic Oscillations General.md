#ClassicalMechanics 
We introduced [[Forced Harmonic Oscillations Approximation| forced harmonic oscillations approximation]] and looked at an example in [[Example of Forced Harmonic Oscillations Approximation]]. Let us solve the equation with an arbitrary force $F(t)$. We start with equations

### Solving for general external potential
$$
\ddot{x}+\omega^2 x = \frac{F(t)}{m}\tag{1}
$$
Then we add by zero giving

$$
\frac{d}{dt}(\dot{x}+i\omega x-i\omega x) +\omega^2 x = \frac{d}{dt}(\dot{x}+i\omega x)-i\omega(\dot{x} + \omega x) = \frac{F(t)}{m}. \tag{2}
$$
Setting $\xi = \dot{x}+i\omega x$ makes equation (2) a 1st order differential equation

$$
\frac{d}{dt}\xi -i\omega \xi = \frac{F(t)}{m}.\tag{3}
$$
The homogenous solution is $\xi(t) = A\exp(i\omega t)$ the inhomogenous solution has form $\xi(t) = A(t)\exp(i\omega t)$. Pluggung the inhomogenous solution in equation (3) and  solving for $\dot{A}(t)$ then multiplying by $\exp(i\omega t)$ gives

$$
\xi = \exp(i\omega t)\left[\int_0^t \frac{F(t')}{m}\exp(-i\omega t') dt' + \xi_0 \right] \tag{4}
$$
where $\xi_0$ is the inital condition for $\xi(0)$. Then $x/\omega = \text{Im}[\xi]$.

### Energy of the system
Using the definiton of energy from [[Energy|energy]] we get that 
$$
E = \frac{m}{2}(\dot{x}^2+\omega^2 x) = \frac{m}{2}|\xi|^2. \tag{5}
$$
Suppose we want to know the energy transfered to the system during the all the time. If we assume that initially the system had zero energy at $t \rightarrow -\infty$ then 
$$
E = \frac{m}{2}\left|\int_{-\infty}^{\infty} \frac{F(t')}{m}\exp(-i\omega t')  dt' \right|^2. \tag{6}
$$
