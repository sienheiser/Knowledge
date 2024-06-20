For two elements from a seperable Hilbert space we know that [[Projection|projection]] and orthogonal complement can be defined. What if we try to project $\psi\in \mathit{H}$ to $\text{span}\{e_i\}_{i\in I}$  with $\{e_i\}\in\mathit{H}$ and $I$ is a countatble index set. Where [[Schauder basis|span]] is defined in the link. We have the following proposition

*Proposition:* Let $\psi\in\mathit{H}$. Let $\{e_i\}_{i\in I}$ be an orthonormal set in $\mathit{H}$ for an at most countable $I$. Then
1. $\psi = \psi_{\perp}+\psi_{||}$ where $\psi_{||}:= \sum_{i\in I} \langle e_i,\psi\rangle e_i$ and $\psi_{\perp}:= \psi-\psi_{||}$.
2. Pythogarol holds $$||\psi||^2 = ||\psi_{\perp}||^2+\sum_{i\in I}|\langle e_i,\psi\rangle||^2 $$
3. For any $\gamma\in \text{span}\{e_i\}$ we have that $||\psi-\gamma||\geq ||\psi_{\perp}||$ with equality iff $\gamma = \psi_{||}$. Note, when we say span we only consider finite linear combinations of the infinite vector space.

Proof: Strategy: Show all of the above is true for a finite set $I$. Then take limit to infinity and show that the above elements are still true. 

Proof for 1. is simple in the finite case since that is true by definiton of [[Projection|projection]].

Proof for 2. in finite case is
$$
\begin{aligned}
||\psi||^2 &= ||\psi_\perp+\psi_{\|}||^2 \\
&=\langle \psi_\perp+\psi_{\|},\psi_\perp+\psi_{\|}\rangle\\

&=\langle \psi_\perp,\psi_\perp\rangle+
\langle \psi_\perp+,\psi_{\|}\rangle+
\langle \psi_{\|},\psi_\perp\rangle+
\langle \psi_{\|},\psi_{\|}\rangle\\

&= ||\psi_\perp||^2+||\psi_\| ||^2
\end{aligned}
$$

Proof for 3. in the fintie case is: Since $\gamma\in\{e_i\}_{i\in I}\implies \gamma = \sum_{i=1}^n\gamma_i e_i$. Then 
$$
\begin{aligned}
||\psi-\gamma||^2 &= ||\psi_\perp+\psi_\|+\gamma||^2 \\

&= ||\psi_\perp||^2+||\psi_\|+\gamma||^2 \\

&= ||\psi_\perp||^2+||\sum_{i=1}^n(\langle e_i,\psi\rangle-\gamma_i)e_i||^2\\

&= ||\psi_\perp||^2+\sum_{i=1}^n|(\langle e_i,\psi\rangle-\gamma_i)|^2\ \\

&\stackrel{1}{\geq} ||\psi_\perp||^2

\end{aligned}
$$
where $\stackrel{1}{\geq}$ is true because the second term in the last equality is positive.

Now that we have proved the proposition for the finite case. We need to proof for the countably infinite case.  Strategy: We split  $\psi = \psi_\perp+\psi_\|$ and show that $\psi_\|$ belongs to the Hilbert space by showing its sequence of partial sums in the limit of inifinity is a [[Cauchy sequence]]. 

Consider integers $n\geq m$ and any $\psi\in \mathit{H}$. Then look at 
$$
\begin{aligned}
||\sum_{i = m}^n\langle e_i,\psi\rangle e_i||^2 &= \sum_{i = m}^n|\langle e_i,\psi\rangle|^2\stackrel{1}{\leq} ||\psi||^2
\end{aligned}
$$
where $\stackrel{1}{\leq}$ is true since we consider a projection of $\psi$. Clearly each term in the sum is positive and the sum is bounded from above. Therefore this implies that the sequence of sums $||\sum_{i = m}^n\langle e_i,\psi\rangle e_i||^2$ is convergent which means that it is a [[Cauchy sequence]]. Therefore $\psi_\|\in\mathit{H}$.


