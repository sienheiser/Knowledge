### 1D infinite well
#### Adjoint
By definiton of [[Self-adjoint and adjoint|adjoint]] for $\psi\in\mathcal{D}_{p^*}$ this implies $\forall\phi\in\mathcal{D}_p\quad\exists\eta\in L^2(\mathbb{R}):\langle\psi,P\phi\rangle = \langle\eta,\phi\rangle$. This means
$$
\int_0^{2\pi}\bar{\psi} (-i)\phi'dx = \int_0^{2\pi}\bar{\eta}\phi dx.
$$
We may rewrite $\eta$ as the derivative of some function $N$ therefore $\eta = N'$. Then by using integration by parts on the RHS of the above equation we get
$$
\begin{aligned}
\int_{0}^{2\pi}(-i\bar{\psi}+\bar{N})\phi'dx &= [\bar{N}\phi]_0^{2\pi}\stackrel{1}{=} 0\\
\int_{0}^{2\pi}(\bar{\psi}+\overline{-iN})\phi'dx &= 0 = \langle\psi-iN,\phi\rangle 
\end{aligned}
$$
where $\stackrel{1}{=}$ is true by definiton of $\phi$. We see $\langle\psi-iN,\phi\rangle=0$. It is clear that $\psi-iN\in\{\phi'|\phi\in\mathcal{D}_P\}^\perp$. What does this mean? Let $A  =\{\phi'|\phi\in\mathcal{D}_P\}$ then $A^\perp = \{\psi\in L^2(\mathbb{R})|\forall \phi'\in A\quad\langle \phi',\psi\rangle = 0\}$. When does $\langle\phi',\psi\rangle = 0$? We can check $0 = \langle\phi',\psi\rangle = \int_0^{2\pi}\phi'\psi dx = [\phi'\psi]^{2\pi}_0-\int_0^{2\pi}\phi\psi'dx =-\int_0^{2\pi}\phi\psi'dx$. This can zero for a arbitrary $\psi\in L^2(\mathbb{R}) \iff \psi(x)=\text{const}$. Therefore since $\psi(x)-iN(x)\in A^\perp$ then $\psi(x) = \text{const}+iN(x)\in \text{AC}(I)$ since $N(x)\in\text{AC}(I)$.

Now we see $\psi\in\mathcal{D}_{p^*}\subseteq\text{AC}(I)$. Furthermore since $p^*:\mathcal{D}_{p^*}\rightarrow L^2(\mathbb{R})|\psi\mapsto -i\psi'$ this is presicely the definiton of an element belonging to [[Sobolov space]] $H^1([0,2\pi])$. There no further refinement we can make therefore $\mathcal{D}_p\subsetneq\mathcal{D}_{p^*}=H([0,2\pi])$. So the momentum operator is not self adjoint.

#### Essentially self adjoint
The momentum operator over this domain could be [[Essentially self adjoint operators|ESAO]]. This means we need to calculate $p^{**}$. We know that $p\subseteq p^{**}\subseteq p^{*}$. Therefore by definiton of $\mathcal{D}_{p^{**}}$ We know $\forall \psi\in\mathcal{D}_{p^{**}}\quad\forall \phi\in\mathcal{D}_{p^{*}} \quad\langle\psi,p^{*}\phi\rangle = \langle p^{**}\psi,\phi\rangle\stackrel{1}{=}\langle p^{*}\psi,\phi\rangle$ where $\stackrel{1}{=}$ is true since $p^{**}\subseteq p^{*}$.

Then 
$$
\begin{aligned}
\langle\psi,p^{*}\phi\rangle &=\langle p^{*}\psi,\phi\rangle\\
\iff \int_{0}^{2\pi}\bar{\psi}(-i)\phi'dx &= \int_{0}^{2\pi}\overline{-i\psi'}\phi dx\\
\iff 0 &= i[\bar{\psi}\phi]_0^{2\pi}
\end{aligned}
$$
we know that $\phi\in H^1([0,2\pi])$ so we cannot say anything about the boundary conditions. Therefore for $[\bar{\psi}\phi]_0^{2\pi}=0$ which means $\psi(0) = \psi(2\pi) = 0$. This implies $D_{p^{**}}=\{\theta\in H^1([0,2\pi])|\theta(0)=\theta(2\pi)=0\}$. So $\mathcal{D}_{p^{**}}\subsetneq\mathcal{D}_{p^{*}}$. Therefore the momentum operator is not essentially self adjoint.

#### Existence of self adjoint
We see that for the 1D inifinite well the given momentum operator is not self-adjoint or essentially self-adjoint. This could mean there exists infinitely many self-adjoint momentum operators. We check the defect indicies $d_+:=\dim \text{ker}(p^*-i)$ and $d_+:=\dim\text{ker}(p^*+i)$ should be equal. If $\psi\in\text{ker}(p^*\mp i)$ then $(p^*\mp i)\psi = 0\iff (-i\psi\mp i\psi=0)\iff \psi(x) =a_{\pm} \exp(\mp x)$ where $a_{\pm}\in\mathbb{C}$. We see that the dimension of both the kernals are equal meaning there exists a self adjoint of $p$. 

