For a [[Simple function|simple function]] $f$ we define 
$$
\int_\mathbb{R}fdP := \sum_{n=1}^{N}f_n\cdot P(\text{preimg}(f_n))
$$

*Observe* 
1. For any [[Characteristic function|charateristic function]] $\chi_\Omega$ for $\Omega\in\sigma(\mathcal{O}_{\mathbb{R}})$ $\int\chi_{\Omega}dP=P(\Omega)$
2. for any $\psi,\phi\in H$
$$
\begin{aligned}
\langle\psi,(\int f dP)\phi\rangle &= \langle\psi,\sum_n f_n P(\Omega_n)\phi\rangle\\
&=\sum_n f_n\langle\psi, P(\Omega_n)\phi\rangle\\
&\stackrel{1}{=}\sum_n f_n\mu_{\psi,\phi}(\Omega_n)\\
&=\int f d\mu_{\psi,\phi}
\end{aligned}
$$ 
where $\stackrel{1}{=}$ is just a [[Borel measure induced by PVM|definiton]].



*Proposition:* The map $\int_\mathbb{R}dP: S(\mathbb{R}):=\{f:\mathbb{R}\rightarrow\mathbb{C}|f\text{ simple }\}\rightarrow\mathcal{L}(H)$ where $f\mapsto \int f dP$ is a [[Linear Maps|linear map]] i.e
$\int f+g dP = \int f dP+\int g dP$ and $\int\alpha f dP=\alpha\int f dP$ with [[Bounded operator norm|operator norm]] ||$\int\cdot dP||= 1$.

*Proof:* ![[proof_proposition.jpg]]