
#QuantumMechanics 
Using the representation of [[Momentum Operator in Position basis|momenutm operator in position basis]] we have 

$$
\left(\langle x'|\hat{p}\right)| p' \rangle = \left(-i\hbar \frac{\partial}{\partial x}\langle x'|\right)|p'\rangle \implies p' \langle x'|p'\rangle = -i\hbar \frac{\partial}{\partial x}\langle x'|p'\rangle. 
$$
The differential equation has solution 

$$
\langle x'|p'\rangle = N \exp(\frac{ip'x'}{\hbar}).
$$
This is the momentum ket representation in position basis. If we take the the Hermitian conjugate of the above equation we get the position ket representation in momentum basis. The normalization factor can be determined by

$$
\langle x'|x \rangle = \int dp \langle x'| p\rangle  \langle p |x\rangle \implies \delta(x'-x) = |N|^2\int dp e^{ip(x'-x)/\hbar} = 2\pi|N|^2\delta(x'-x).
$$
This gives $N = 1/\sqrt{2\pi\hbar}$.