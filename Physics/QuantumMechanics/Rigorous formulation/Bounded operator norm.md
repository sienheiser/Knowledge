Given map $A$ defined in [[Bounded maps|bounded maps]].

*Definiton:* The operator norm of a bounded operator is 
$$
||A|| = \sup_{||f||=1}||Af||_W
$$

### Example

Suppose we have [[Banach space]] $W$. We look at the identity map 
$$
\begin{aligned}
\text{id}_W:&W\rightarrow W\\
&f\mapsto f
\end{aligned}
$$
Therefore $||\text{id}_W|| = \sup_{||f||_W=1}||\text{id}_Wf|| = \sup_{||f||_W=1}||f|| = 1$.

### Counter example

Let $W = C^0([0,1])$ be the set of all function on the interval $[0,1]$ that are continuos. Defining the norm 
$$
||f||_\infty := \sup_{x\in[0,1]}|f(x)|
$$
one can show: $(W,||\cdot||_\infty)$ is complete.

define a map $P:C^1([0,1])\rightarrow C^0([0,1])$ which $C^1([0,1])\ni f\mapsto f'$ where $f'$ is the derivative. Clearly $C^1([0,1])\subseteq C^0([0,1])$ meaning it is a subvector space which can inherit the norm $||\cdot||_\infty$.

Claim: $P$ is not bounded. 
Proof: Consider the sequence $f:\mathbb{N}^*\rightarrow C^1([0,1])$ where $f_n(x):=\sin(2\pi n x)$. Clearly $f_n$ is one time continuosly differentiable. We see $||f_n||_\infty = 1$. Then $P(f_n)(x) = 2\pi n\cos(2\pi n x)$. Clearly, $P(f_n)$ is a continuous function. We see $||P(f_n)(x)||_\infty = 2\pi n$. 

Therefore
$$
\begin{aligned}
||P|| &:= \sup_{f\in C^1} \frac{||P f||_\infty}{||f||_\infty}\\
&\geq \sup_{f\in{f_n}\subseteq C^1}\frac{||P f||_\infty}{||f||_\infty}\\
&= \sup_{n\in \mathbb{N}^*}\frac{||P f_n||_\infty}{||f_n||_\infty}\\
&= \sup_{n\in \mathbb{N}^*}2\pi n\\
\end{aligned}
$$
which is not bounded.