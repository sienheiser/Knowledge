Consider a bounded linear map which is [[Physics/QuantumMechanics/Rigorous formulation/Dense|densely]] defined on 

$$
A:\mathcal{D}_A\rightarrow W
$$
where $\mathcal{D}_A\subseteq V$ with $V$ being a norm space and $W$ a [[Banach space]]. Question does there exist an extenstion of $A$ denoted $\hat{A}$ which $\hat{A}:V\rightarrow W$ and is bounded.

BLT theorem: There is a unique such extension of $A$ to a bounded map $\hat{A}$.

In other words we may (and alwats will) extend a bounded linear map to the entire normed space at hand.

Proof: *Defining candidate map*: Let $A\in \mathcal{L}(\mathcal{D}_A,W)$ where $\mathcal{L}$ was defined in [[Theorem of Banach space of linear bounded maps|here]] and $\mathcal{D}_A\subseteq V$. Let $f\in V$ and sequence $\{f_n\}\subseteq \mathcal{D}_A$ where $\lim_{n\rightarrow \infty} f_n = f$ because $\overline{\mathcal{D}_A} = V$ where $\overline{\mathcal{D}_A}$ is closure?????. 
Then $f_n$ is certainly Cauchy because of convergence. Then $Af_n$ is again Cauchy sequence since $A$ is [[Bounded maps|bounded]].  Furthermore, since $W$ is a Banach space
$$
\lim_{n\rightarrow \infty} A_nf\in W
$$
Now define the extenstion $\hat{A}$ as the map 
$$
\begin{aligned}
\hat{A}:&V\rightarrow W\\
&f\mapsto \hat{A}f:= \lim_{n\rightarrow \infty}(A f_n)

\end{aligned}
$$

*Showing it is an extension:* Next question to answer. If the defined extension an extension?  Let $\alpha\in\mathcal{D}_A$. Then $f_n :=\alpha$ is a sequence in $\mathcal{D}_A$, that converges to $\alpha$. Then 
$$
\hat{A}(\alpha):= \lim_{n\rightarrow \infty}(A f_n) = \lim_{n\rightarrow \infty} (A\alpha) = A(\alpha)
$$

*Showing it is a linear map*
$$
\begin{aligned}
\hat{A}(f)+\hat{A}(g) &= \lim_{n\rightarrow \infty} Af_n + \lim_{n\rightarrow \infty} Ag_n\\
&=|F_n:= f_n+g_n,\quad F_n\rightarrow f+g|\\
&= \hat{A}(f+g)
\end{aligned}
$$
Similar for $\lambda\hat{A}(f) = \hat{A}(\lambda f)$.

*Remains to show:*
1. $\hat{A}f:= \lim_{n\rightarrow\infty}Af_n$ is well defined for $\mathcal{D}_A\ni f_n\rightarrow f\in V$. Do this by choosing another sequence $g_n$ which converges to $f$ and show that $\lim_{n\rightarrow \infty}Ag_n = \lim_{n\rightarrow \infty}A f_n$.
2. $\hat{A}$ is bounded and that $||\hat{A}|| = ||A||$.