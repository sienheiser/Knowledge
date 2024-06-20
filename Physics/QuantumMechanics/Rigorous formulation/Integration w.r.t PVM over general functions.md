*Definiton:* Let $f$ be a [[Measureable maps|measureable]] function $f:\mathbb{R}\rightarrow \mathbb{C}$. Then we define the lienar map 
$$
\int_{\mathbb{R}}fdP:\mathcal{D}_{\int_{\mathbb{R}}fdP}\subseteq H\rightarrow H
$$
on the dense linear subset 
$$
\mathcal{D}_{\int_{\mathbb{R}}fdP}:= \{\psi\in H|\int |f|^2d\mu_\psi <\infty\}
$$
where $\mu_\psi$ is defined [[Borel measure induced by PVM|here]]. The elements $\psi$ is mapped as follows 
$\psi\mapsto(\int_\mathbb{R}fdP)(\psi):=\lim_{n\rightarrow \infty}[(\int f_ndP)\psi]$
where the 
$$
f_n := \chi_{\{x\in\mathbb{R}:|f(x)|\leq n\}}f
$$
and a sequence that 
$$
\{f_n\}_{b\in\mathbb{N}}\subseteq B(\mathbb{R})
$$

*Proof:* Show that $f_n$ is a [[Cauchy sequence]] in $L^2(\mathbb{R})$. Then shows that $(\int f_ndP)\psi$


*Properties:*
1. $(\int f dP)^* = \int \bar{f}dP$
2. $\int (\alpha f+g)dP \supseteq \alpha\int fdP+\int g dP$ where the domain of RHS is $\mathcal{D}_{\int_\mathbb{R}(|f|+|g|)dP}$
3. $\int (f\cdot g)dP\supseteq\int f dP\circ \int g dP$ where the domain of the RHS is $\mathcal{D}_{\int f dP}\cap \mathcal{D}_{\int g dP}$.