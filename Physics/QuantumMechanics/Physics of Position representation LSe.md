#QuantumMechanics 

The position representation of LSe has been [[Position Representation of LSe|derived]]. We know discuss the physics of the equation now. The situation we consider is the following: The scattering potential has limited range and we observe the scattered wave function far from the scattering potential. From a physical stand point of view, scattering potential are usually other particles. It is not possible to place a detector near a particle. Therefore we can approximate the function $\frac{1}{|\vec{x}-\vec{x}'|}$ where $\vec{x}$ is point in space that we observe the wave function and $\vec{x}'$ points towards the distribution of the wave function. If $x>>x'$ which are the magnitudes of their respective vectors. Then we get the following [[Approximating Source to Point Vector|approximation]]. As a result the position representation of LSe can be written as

$$
\langle \vec{x}|\psi^{(\pm)}\rangle = \langle\vec{x}|i\rangle+ \frac{2m}{\hbar^2}\frac{\exp(\pm ik/\hbar)}{x}\int d^3x'-\frac{1}{4\pi}\exp(\mp i \vec{k}'\cdot\vec{x}'/\hbar) V(\vec{x}')\langle x'|\psi^{(\pm)}\rangle
$$
$$
= \frac{1}{L^{3/2}}\left[e^{i\vec{k}\cdot\vec{x}}    +\frac{\exp(\pm ik/\hbar)}{x} f(\vec{k},\vec{k}')\right].
$$
where we set $|i\rangle = | \vec{k}\rangle$.  The form above shows that our scattered state is a sum of the initial state plus a radial wave with amplitude 