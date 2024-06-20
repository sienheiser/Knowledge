*Theorem:* Given a norm vector space $V$ and a [[Banach space]] $W$. The set 
$$
\mathcal{L}(V,W) := \{A:V\rightarrow W | A\quad\text{is a bounded linear map}\}
$$
is a Banach space if equipped with the operator 
$$
||\cdot||_{\mathcal{L}(V,W)}.
$$

Proof: First show that the set satifies the vector space axioms. Next we need to show $(\mathcal{L}(V,W),||\cdot||_{\mathcal{L}})$ is complete. Strategy is to  assume $A_n$ is a [[Cauchy sequence]] in $\mathcal{L}(V,W)$
1. Construct a candidate for the limit of this sequnce
2. Show that $A$ is linear
3. Show that $A$ is bounded
4. Show that $A_n\rightarrow A$

Step 1: Observe if $A_n$ is Cauchy in $\mathcal{L}$ then for all $f\in V$ the sequence $\{A_n f\}_{n\in\mathbb{N}}\subseteq W$ is also a Cauchy sequence. To se this we know that 
$$
\forall \epsilon>0 \quad \exists N \in \mathbb{N}^*\quad \forall n,m\geq N:||A_n-A_m|| <\epsilon
$$
Therefore taking the sequence 
$$
\begin{aligned}
\forall f\in V:||A_n f-A_m f|| &= ||(A_n -A_m)f||\\
&\leq ||A_n-A_m ||\cdot ||f||\\
&< \epsilon ||f||
\end{aligned}
$$
Therefore we have shown the existence of $\epsilon ||f||$. Since we know $(W,||\cdot||)$ is Banach:
$$
\lim_{n\rightarrow \infty} A_n f 
$$
converges by definiton. We define the candidate map 
$$
\begin{aligned}
A:&V\rightarrow W\\
&f\mapsto \lim_{n\rightarrow\infty}(A_nf)

\end{aligned}
$$ 

Step 2: Show $A$ is linear 
$$
\begin{aligned}
A(f+g)&:= \lim_{n\rightarrow \infty} (A_n(f+g)) \\
&\stackrel{1}{=} \lim_{n\rightarrow \infty} (A_n f+ A_n g)\\
&\stackrel{2}{=} \lim_{n\rightarrow \infty} A_n f+ \lim_{n\rightarrow \infty} A_n g\\
&= Af+Ag
\end{aligned}
$$
where $\stackrel{1}{=}$ is possible because operator is linear and $\stackrel{2}{=}$ is possible because we can view the addition between $f$ and $g$ as a $+_W:W\times W\rightarrow W$. Taking the limit $\lim_{n\rightarrow\infty}M(F_n) = M(\lim_{n\rightarrow\infty} F_n)$ is only possible if the map is continous topologically. A similar thing can be done for the scalar multiplication.

Step 3: A is bounded. 
$$
\begin{aligned}
\forall f\in V\quad ||A f|| &= ||\lim_{n\rightarrow\infty} (A_n f)||\\
&\stackrel{!}{=}\lim_{n\rightarrow\infty}||A_n f ||\\
&\leq \lim_{n\rightarrow\infty}||A_n||\cdot||f|| 
\end{aligned}
$$
where $\stackrel{!}{=}$ is only possible if $||\cdot||$ is continuous.  We need to show that $||A_n||$ is finite. Since $||A_n||$ is a [[Cauchy sequence]] we know that 
$$
\forall \epsilon>0 \quad \exists N \in \mathbb{N}^*\quad \forall n,m\geq N:||A_n-A_m|| <\epsilon
$$
Therefore this implies
$$
\forall \epsilon>0 \quad \exists N \in \mathbb{N}^*\quad \forall n\geq N:||A_n-A_N|| <\epsilon
$$

Now $||A_n-A_N|| \geq ||A_n||-||A_N||$  therefore
$$
\forall \epsilon>0 \quad \exists N \in \mathbb{N}^*\quad \forall n\geq N:||A_n|| <\epsilon + ||A_N||
$$
Hence $||A_n||$ is finite.

Step 4: Finally show that the Cauchy sequence converges against $A$. Since $A_n$ is Cauchy
$$
\forall \epsilon>0 \quad \exists N \in \mathbb{N}^*\quad \forall n,m\geq N:||A_n-A_m|| <\epsilon
$$
Now we can use the estimate $||A_n-A_m||\geq ||(A_n-A_m)f||/||f||$ for any $f$ which gives
$$
\forall \epsilon>0 \quad \exists N \in \mathbb{N}^*\quad \forall n,m\geq N:||(A_n-A_m)f|| <||f||\epsilon
$$
Now taking the limit of $m\rightarrow \infty$ of the above expression gives

$$
\begin{aligned}
&\lim_{m\rightarrow \infty}||(A_n-A_m)f|| < \epsilon||f||\\
&\implies \lim_{m\rightarrow \infty}||A_nf-A_mf|| < \epsilon||f||\\
&\implies ||A_nf-\lim_{m\rightarrow \infty}A_mf|| < \epsilon||f||\\
&\implies ||A_nf-Af|| < \epsilon||f||\\
\end{aligned}
$$

This finally gives
$$
\forall \epsilon>0 \quad \exists N \in \mathbb{N}^*\quad \forall n\geq N:\forall f\in V:\frac{||A_nf-Af||}{||f||} <\epsilon
$$