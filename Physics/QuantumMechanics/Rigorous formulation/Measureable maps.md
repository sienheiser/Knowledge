

*Definiton:* Let $(M,\sigma_M),(N,\sigma_N)$ be [[Sigma algebra|measureable spaces]]. A map $f:M\rightarrow N$ is called **measurable** w.r.t $\sigma_M and \sigma_N$ if $\forall A\in\sigma_N: \text{preim}_f(A)\in\sigma_M$.

*Lemma:* To show that $f$ is measureable it suffices to check whether $\forall A\in E: \text{preim}(A)\in\sigma_M$ where $E$ is a [[Generating sigma algebra|generating set]] for $\sigma_N$.

*Corollary:*:
1. Any continous map w.r.t to [[Borel sigma algebra|Borel sigma aldebras]] is measureable. This is true because the sigma algebras are defined using topologies. Continuity in topology for a map is the same as measurerable.
2. Any monotonous map $f:\mathbb{R}\rightarrow\mathbb{R}$ w.r.t is measureable w.r.t [[Borel sigma algebra]].

*Theorem:* The composition $f\circ g:A\rightarrow C$ of measureable maps 
$$
\begin{aligned}
f:B&\rightarrow C\\
g:A&\rightarrow B
\end{aligned}
$$ 
 is again measureable.
 *Proof*:?????