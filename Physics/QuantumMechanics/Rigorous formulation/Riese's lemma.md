Before we state the lemma lets build up the quesiton the lemma answers. Consider $\lambda\in H$ where $H$ is a Hilbert space. Suppose we have map
$$
\begin{aligned}
l_{\lambda}:&H\rightarrow \mathbb{C}\\
&\alpha\mapsto\langle\lambda,\alpha\rangle
\end{aligned}
$$
We see the map is bounded since
$$
\begin{aligned}
||l_\lambda|| &= \sup_{\alpha\in H}\frac{|l_\lambda(\alpha)|}{||\alpha||}\\
&=\sup_{\alpha\in H}\frac{|\langle \lambda,\alpha\rangle|}{||\alpha||}\\
&\stackrel{1}{\leq}\sup_{\alpha\in H}\frac{|| \lambda||\cdot ||\alpha||}{||\alpha||}\\
&=\sup_{\alpha\in H}\frac{|| \lambda||}{1} \stackrel{2}{<} \infty\\
\end{aligned}
$$
where $\stackrel{1}{\leq}$ is the [[Cauchy-Scwarch inequality]] and $\stackrel{2}{<}$ is true because $\lambda\in H$. Therefore $l_\lambda\in\mathcal{L}(H,\mathbb{C}):= H^*$. 

*Question:* Can any $l\in H^*$ be uniquely written as $l=l_\lambda$?
Riese's lemma: Yes!

*proof:* Case 1: $l = 0_{\mathbb{C}}$: then take $\lambda = 0$.
Case 2: $l\neq 0$: then kernal of $l$ which is defined as
$$
\text{ker}(l) = \{\psi\in H|l(\psi) = 0\}.
$$

We may define the otrhogoal complement of the $\text{ker}(l)$ as $(\text{ker}(l))^\perp$. We may then decompose the Hilbert space as
$$
H = \text{ker}(l) \oplus (\text{ker}(l))^\perp
$$
In general $\text{ker}(l)$ may contain many more vectors other than $0_H$. Wlog we can choose $\xi\in(\text{ker}(l))^\perp$ where $||\xi|| = 1$. Then take $\lambda = \overline{l(\xi)}\xi\in (\text{ker}(l))^\perp\subseteq H$.

We now show $l_\lambda(\alpha)-l(\alpha) = 0$.
$$
\begin{aligned}
l_\lambda(\alpha)-l(\alpha) &= \langle \overline{l(\xi)}\xi,\alpha \rangle - l(\alpha)\\
&\stackrel{1}{=}\langle \xi,l(\xi)\alpha \rangle - \langle \xi,\xi \rangle l(\alpha)\\
&\stackrel{2}{=}\langle \xi,l(\xi)\alpha -\xi l(\alpha) \rangle \\
&\stackrel{3}{=} 0\\
\end{aligned}
$$

where $\stackrel{1}{=}$ is true becuause the inner product is antilinear in the first slot and $\langle \xi,\xi\rangle = 1$, $\stackrel{2}{=}$ is true because inner product is linear in second slot and $\stackrel{3}{=}$ is true because $\xi\in(\text{ker}(l))^\perp$ and $l(\xi)\alpha -\xi l(\alpha) \in \text{ker}(l)$ because $l(l(\xi)\alpha -\xi l(\alpha) ) = l(\xi)l(\alpha) - l(\xi)l(\alpha) = 0$. The inner product between an element of the kernal and an element belonging to its orthogonal complement is zero.