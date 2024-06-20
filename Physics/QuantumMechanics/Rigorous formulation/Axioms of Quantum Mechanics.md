*Axiom 1:* For every quantum system there is associated a [[Banach space|complex hilbert space]] $(\mathit{H},+,\cdot,\langle\cdot|\cdot\rangle)$ which is equipped with a [[Sesqui-linear map|sesqui-linear map]]. The [[States|states]] of the system are all [[Positive|positive]] [[Trace-class|trace-class]] [[Linear Maps|linear maps]] $\rho:\mathit{H}\rightarrow\mathit{H}$ for which 
$$
\text{Tr} \rho = 1
$$


*Axiom 2:* The observables of a quantum system are [[Self-adjoint and adjoint|self-adjoint]] [[Linear Maps|linear maps]] $A:\mathcal{D}_A\rightarrow\mathit{H}$ where the set $\mathcal{D}_A$ is defined [[Physics/QuantumMechanics/Rigorous formulation/Dense|dense]].

*Axiom 3:* The probability that a measurement of an observable $A$ on a system is in the state $\rho$ yeilds a result in the [[Borel set]] $E\subseteq \mathbb{R}$ is given by
$$
\mu^A_\rho(E):= \text{Tr}(P_A(E)\circ \rho)
$$
where $P_A:\text{Borel}(\mathbb{R})\rightarrow \mathcal{L}(\mathit{H})$ (where $\mathcal{L}$ is defined [[Theorem of Banach space of linear bounded maps|here]]) is the unique projection valued measure that is associated with a [[Self-adjoint and adjoint|self-adjoint]] map $A$ according to the [[Spectral theorem|spectral theorem]] 
$$
A = \int_{-\infty}^{\infty}\lambda dP_A(\lambda)
$$

*Axiom 4* (Unitary dynamics): during time interval $(t_1,t_2)$ during which no measurement occurs the state $\rho(t_2)$ and $\rho(t_1)$ are related through 
$$
\rho(t_2) = \mathcal{U}(t_2-t_1)\rho(t_1)\mathcal{U}^{-1}(t_2-t_1)
$$
where $\mathcal{U} = \exp(\frac{-i}{\hbar} H t)$ where $H$ is the energy observable. For a given function $f:\mathbb{R}\rightarrow \mathbb{C}$ and [[Self-adjoint and adjoint|self-adjoint]] linear map $A$
$$
f(A) = \int_{-\infty}^{\infty}f(\lambda)dP_A(\lambda)
$$


*Axiom 5 (Projective dynamics/Wavefunction collapse):* When a measurement is made at $t_m$. Then the state immediately after the measurement $\rho_{\text{after}}$ is related to the state immediately before the measurement of a observable $A$ is 
$$
\rho_{\text{after}}:= \frac{P_A(E)\rho_{\text{before}}P_A(E)}{\text{Tr}(\text{numerator})}
$$
where $E$ is the smallest [[Borel set]] in which the actual outcome of the measurement happened.