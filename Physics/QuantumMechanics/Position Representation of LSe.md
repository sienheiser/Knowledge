#QuantumMechanics 



We have derived the [[Lippmann-Schwinger equation (LSe)]]. To find its form in position representation we include the position basis kets in the equation giving 

$$
\langle\vec{x}|\psi^{(\pm)}\rangle = \langle\vec{x}|\phi\rangle+ \left\langle\vec{x}|\frac{1}{E-\hat{H}_0 \pm i\epsilon}\hat{V}|\psi^{(\pm)}\right\rangle.
$$

If we insert the position eigenkets we get

$$
\langle\vec{x}|\psi^{(\pm)}\rangle = \langle\vec{x}|\phi\rangle+ \int d^3x'\left\langle\vec{x}|\frac{1}{E-\hat{H}_0 \pm i\epsilon}|\vec{x}'\right\rangle \langle \vec{x}'| \hat{V}|\psi^{(\pm)}\rangle = \langle\vec{x}|\phi\rangle+ \frac{2m}{\hbar^2}\int d^3x'G^{(\pm)}(\vec{x},\vec{x}';E) \langle \vec{x}'| \hat{V}|\psi^{(\pm)}\rangle
$$
where 
$$
G^{(\pm)}(\vec{x},\vec{x}';E) = \frac{\hbar^2}{2m}\left\langle\vec{x}|\frac{1}{E-\hat{H}_0 \pm i\epsilon}|\vec{x}'\right\rangle.
$$

We have to find the position representation of  $G^{(\pm)}(\vec{x},\vec{x}';E)$. This can be done by introducing the momentum state kets giving

$$
G^{(\pm)}(\vec{x},\vec{x}';E) =\int d^3p \frac{\hbar^2}{2m}\langle\vec{x}|\frac{1}{E-\hat{H}_0 \pm i\epsilon}|\vec{p}\rangle\langle \vec{p}|\vec{x}'\rangle.
$$

Since $|\vec{p}\rangle$ are eigenkets of $\hat{H}_0$ we can move it to the other side and get $\langle \vec{x}|\vec{p}\rangle$. Using [[Position and Momentum Ket Representations| position and momentum ket representations]] we obtain

$$
G^{(\pm)}(\vec{x},\vec{x}';E) =\int d^3p \frac{\hbar^2}{2m}\langle\vec{x}|\vec{p}\rangle\frac{1}{E-H_0 \pm i\epsilon}\langle \vec{p}|\vec{x}'\rangle = \int \frac{d^3p}{(2\pi\hbar)^3} \exp(\frac{i\vec{p}}{\hbar}\cdot(\vec{x}-\vec{x}'))\frac{1}{E-H_0 \pm i\epsilon}.
$$

Then $\exp(\frac{i\vec{p}}{\hbar}\cdot(\vec{x}-\vec{x}'))$ can be rewritten as $\exp(\frac{ip}{\hbar}|\vec{x}-\vec{x}'|\cos(\theta))$. The integration measure can be changed to $d^3p=2\pi p'^2 dp'd(\cos(\theta))$. After integrating out the $d(\cos(\theta))$ we get

$$
G^{(\pm)}(\vec{x},\vec{x}';E) =\frac{1}{8\pi} \frac{1}{i|\vec{x}-\vec{x}'|}\int dp' p'\left[\frac{e^{-ip'|\vec{x}-\vec{x}'|}-e^{ip'|\vec{x}-\vec{x}'|}}{p^2-p'^2\pm i\epsilon}      \right]
$$

where $p'^2$ is the eigen value of the free Hamiltonian, $p^2$ is the energy of the particle and the constant $\hbar/2m$ is aborbed into $\epsilon$. Using [[Complex Contour Integrals|complex contour integrals]] we get 

$$
G^{(\pm)}(\vec{x},\vec{x}';E) = -\frac{1}{4\pi}\frac{\exp(\pm ip|\vec{x}-\vec{x}'|/\hbar)}{|\vec{x}-\vec{x}'|}
$$
which is essentially a [[Green's Function| Green's function]]. Therefore the position representation of the LSe equation is

$$
\langle \vec{x}|\psi^{(\pm)}\rangle = \langle\vec{x}|i\rangle+ \frac{2m}{\hbar^2}\int d^3x'-\frac{1}{4\pi}\frac{\exp(\pm ip|\vec{x}-\vec{x}'|/\hbar)}{|\vec{x}-\vec{x}'|} \langle x'|\hat{V}|\psi^{(\pm)}\rangle
$$

We consider a special class of potentials known as local potentials which are diagonal in position representation meaning

$$
\langle \vec{x}'|\hat{V}|\vec{x}''\rangle = \delta(\vec{x}'-\vec{x}'')V(\vec{x}')
$$
This finally gives,

$$
\langle \vec{x}|\psi^{(\pm)}\rangle = \langle\vec{x}|i\rangle+ \frac{2m}{\hbar^2}\int d^3x'-\frac{1}{4\pi}\frac{\exp(\pm ip|\vec{x}-\vec{x}'|/\hbar)}{|\vec{x}-\vec{x}'|} V(\vec{x}')\langle x'|\psi^{(\pm)}\rangle
$$



