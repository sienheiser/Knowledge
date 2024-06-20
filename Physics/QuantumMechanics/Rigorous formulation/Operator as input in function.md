*Definiton:* Let $A$ be spectrally decomposable i.e
$$
\exists \quad\text{PVM}\quad P\quad A = \int \text{id}_{\mathbb{R}}dP. 
$$

Then if $f$ is any measurable function $f:\mathbb{R}\rightarrow\mathbb{R}$ we define the operator 
$$
f(A):= \int f(\lambda)P(d\lambda):=\int(f\circ\text{id}_{\mathbb{R}})dP.
$$

So $f(A):\mathcal{D}_{\int f dP}\rightarrow H$ where $\mathcal{D}_{\int f dP}:=\{\psi\in H|\int|f|^2d\mu_\psi\}$ where $\mu_\psi$ is defined [[Borel measure induced by PVM|here]].


*Examples*:
1. $\exp(A) := \int_{\mathbb{R}}e^{\lambda}P(d\lambda)$ which is self-adjoint
2. $\exp(iA) := \int_{\mathbb{R}}e^{i\lambda}P(d\lambda)$ which is unitary
