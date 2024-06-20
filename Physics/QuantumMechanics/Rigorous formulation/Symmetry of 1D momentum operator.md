### 1D infinite well
We want to check if $P\psi = -i\partial_x\psi$ is symmetric on domain $\mathcal{D}_P:=\{\psi\in C^1(I)|\psi(0)=\psi(2\pi) = 0\}$. [[Symmetric operator|By definiton]]
$$
\begin{aligned}
\langle \phi,P\psi\rangle &= \langle P\psi,\phi\rangle\quad\forall \psi,\phi\in\mathcal{D}_{A}\\
\end{aligned}
$$

The right hand side of the above equation can be written as
$$
\begin{aligned}
\langle P\psi,\phi\rangle &= \int_0^{2\pi}\overline{-i\psi'(x)}\phi(x)dx\\
&=i[\bar{\psi}(x)\phi(x)]_0^{2\pi}-i\int_0^{2\pi}\bar{\psi}(x)\phi(x)dx\\
&\stackrel{1}{=}\int_0^{2\pi}\bar{\psi}(x)(-i)\phi'(x)dx\\
&=\langle\psi,P\phi\rangle.
\end{aligned}
$$
where $\stackrel{1}{=}$ is true because $\psi,\phi\in\mathcal{D}_P$. We see the momentum operator is symmetric.

### 1D ring

