#QuantumMechanics 


According to wikipedia the LSe equation can be viewed as the [[Schrodinger equation]] with boudary conditions of scattering already built-in.  

### Derivation of LSe 
Imagine a particle encounters a scattering potential. Before the particle encountered the scattering potential it could be described by the state ket $|\phi\rangle$ and free particle Hamiltonian $\hat{H}_0$. If partilce has energy $E$ then $\hat{H}_0|\phi\rangle = E|\phi\rangle$. 

Now the particle undergoes elastic scattering when the scattering potential is introduced. This gives a new Hamiltonian $\hat{H} = \hat{H}+\hat{V}$ and new state ket $|\psi\rangle$, with $\hat{H}|\psi\rangle = E|\psi\rangle$. The energy is the same because of elastic scattering. The new Hamiltonian is $\hat{H}=\hat{H}_0+\hat{V}$. We obtain the following 
$$
(\hat{H}_0+\hat{V})|\psi\rangle = E|\psi\rangle \implies (E-\hat{H}_0)|\psi\rangle = \hat{V}|\psi\rangle.
$$
The equation after the implication is an inhomogenous differential equations. It has a homogenous solutions and a particular solutions. The homogenous solution $|\psi\rangle_h$ satifies 

$$
(E-\hat{H}_0)|\psi\rangle_h = 0
$$
this means $|\psi\rangle_h = |\phi\rangle$ which is just the free particle solution. The particular solution can be found by

$$
(E-\hat{H}_0)|\psi\rangle_p = \hat{V}|\psi\rangle \implies |\psi\rangle_p = \frac{\hat{V}}{(E-\hat{H}_0)}|\psi\rangle.
$$

However, there is a singularity when $|\psi\rangle$ has energy $E$. To deal with this we introduce $\pm i\epsilon$ in the denominator. This yields the LSe equation
$$
|\psi^{(\pm)}\rangle = |\psi\rangle_h+|\psi\rangle_p = |\phi\rangle+ \frac{\hat{V}}{E-\hat{H}_0+\pm i\epsilon}|\psi^{(\pm)}\rangle
$$
where the plus sign corresponds to the retarded solution and minus sign correponds to the advanced solutions.
