We defined $\mathcal{l}^2(\mathbb{N})$ [[Classification of infinite Hilbert space|here]]. Suppose we have another seperable Hilbert space $(\mathit{H},+,\cdot,\langle\cdot,\cdot\rangle)$. We show that 
$(\mathit{H},+,\cdot,\langle\cdot,\cdot\rangle)\cong_{\text{Hilbert}}(\mathcal{l}^2(\mathbb{N}),+,\cdot,\langle\cdot,\cdot\rangle)$ where each Hilbert space has their own inner product.
Proof: Need to show that there exists a bounded linear map 
$$
\mathcal{U}:\mathit{H}\rightarrow\mathcal{l}^2(\mathbb{N})
$$
such that $||\mathcal{U}\psi|| = ||\psi||$. We may construct a map such as $\psi\mapsto \{\langle e_n,\psi\rangle\}$ for all $\psi\in\mathit{H}$ where the set $\{\langle e_n,\psi\rangle\}$ is a sequence of complex numbers. We see that the norm of $||\{\langle e_n,\psi\rangle\}||^2 = \sum_{n=1}^{\infty}|\langle e_n,\psi\rangle|^2 < \infty$ because $||\psi||$ is finite. Remember these are norms in two different spaces. We may define the inverse map as
$$
\begin{aligned}
\mathcal{U}^{-1}:&\mathcal{l}^2(\mathbb{N})\rightarrow \mathit{H}\\
&\{a_n\}\mapsto \sum_{n=1}^\infty a_n e_n.
\end{aligned}
$$

Then we see that $\mathcal{U}^{-1}\circ\mathcal{U}(\psi) = \sum_{n=1}^{\infty}\langle e_n,\psi\rangle e_n =\psi$. 

We show that the candidate map is unitary by showing
$$
||\mathcal{U}\psi||^2_{\mathcal{l}^2(\mathbb{N})} =  ||\psi||^2_{\mathit{H}}.
$$

Start with 
$$
\begin{aligned}
||\psi||^2 &= ||\sum_{n=1}^{\infty} \langle e_n,\psi\rangle e_n||^2\\
&\stackrel{1}{=} \lim_{N\rightarrow \infty}||\sum_{n=1}^{N} \langle e_n,\psi\rangle e_n||^2\\
&\stackrel{2}{=}\lim_{N\rightarrow \infty}\sum_{n=1}^{N}|| \langle e_n,\psi\rangle e_n||^2\\
&\stackrel{3}{=}\lim_{N\rightarrow \infty}\sum_{n=1}^{N}| \langle e_n,\psi\rangle|^2 ||e_n||^2\\
&\stackrel{4}{=}\lim_{N\rightarrow \infty}\sum_{n=1}^{N}| \langle e_n,\psi\rangle|^2\\
&\stackrel{5}{=}||\mathcal{U}\psi||\\
\end{aligned}
$$
where $\stackrel{1}{=}$ is because of the continuty of the norm, $\stackrel{2}{=}$ is because of ON-basis of seperable Hilbert space, $\stackrel{3}{=}$ is just seperating the complex number from the vector element, $\stackrel{4}{=}$ because of ON-basis and $\stackrel{5}{=}$ is the definiton of the norm in $\mathcal{l}^2(\mathbb{N})$.