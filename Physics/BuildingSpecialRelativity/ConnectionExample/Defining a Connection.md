



## Introduction
We have defined an example of a [[Making a Fibre Bundle|fibre bundle]]. The fibre bundle is $(C^1\times\mathbb{R},\pi,C^1)$ where $\mathbb{R}$ is the fibre. The goal of this note is to define make an [[Ehresmann Connection]] on the fibre bundle. 

To do this we will first define for all points in $C^1\times\mathbb{R}$ a vertical tangent at the point. Then look at a vertical tangent point using charts to see what types of tanget vectors belong to it. After that, the we will define the vertical sub-bundle $V C^1\times\mathbb{R}$ and study how it looks using the cartesian chart.

We will also repeate the same steps in the previous paragraph but for horizontal tangent space, and a horizontal sub-bundle $HC^1\times\mathbb{R}$.

## Vertical Sub-bundle
### Vertical tangent space
Before we can define the vertical sub-bundle $VC^1\times\mathbb{R}$ of the fibre bundle, we have to define the vertical tangent space at $p$, $V_p C^1\times\mathbb{R}$ for all $p\in C^1\times\mathbb{R}$. Take a $p\in C^1\times\mathbb{R}$, we define 
$$
V_p C^1\times\mathbb{R} = \text{ker}(\pi_{*p}) :=\{X\in T_p C^1\times\mathbb{R}:\pi_{*p}(X) = 0\}
$$

where $\pi_{*p}$ is the push forward map of $\pi$ at $p$. To understand what type of tangent vector belong to $V_p C^1\times\mathbb{R}$ let $\gamma:\mathbb{R}\rightarrow C^1\times\mathbb{R}$ where $\gamma(0)=p$ and $f\in C^\infty(C^1)$ which is the set of all infinitely differentiable functions on $C^1$. Then 
$$
\begin{aligned}
\pi_{*p}(X_{\gamma,p})f &= X_{\gamma,p}(f\circ\pi) \\
&=: (f\circ\pi\circ\gamma)'(0)\\
&\stackrel{?}{=} 0
\end{aligned}
$$
Where the last question is asking when it equals to zero. If $\forall \lambda\in\mathbb{R}:\pi\circ\gamma(\lambda) = constant$  then $\pi_{*p}(X_{\gamma,p})$ = 0. Meaning for all $X\in V_pC^1\times\mathbb{R}$, $X$ must point along the fibre $\text{preim}_{\pi}(\{\pi(p)\})$.

#### Vertical tangent space chart

![[TangentBundle.jpg]]
Now that we know that all $X\in V_pC^1\times\mathbb{R}$ point along the fibre at $\pi(p)$ we may study $X$ using charts. Suppose we have a curve $\gamma:\mathbb{R}\rightarrow C^1\times\mathbb{R}$ that moves along the fibre $\text{preim}_{\pi}(\{\pi(p)\})$ (the yellow line in the figure). Then using the cartesian chart $x$ of $(C^1\times\mathbb{R},\pi,C^1)$ the curve $\gamma$ has form 
$$
x(\gamma(\lambda))=(r\cos \alpha,r\sin\alpha,z(\lambda))
$$
where $r$ is a positive real number, $\alpha\in [0,2\pi)$ and $z$ is a smooth funciton that depends on $\lambda$. Then the vector $X_{\gamma,\gamma(\lambda)}$ has components
$$
X_{\gamma,\gamma(\lambda)} = (x^i\circ\gamma)'(\lambda)(\frac{\partial}{\partial x^i})_{\gamma(\lambda)}=z'(\lambda)(\frac{\partial}{\partial x^3})_{\gamma(\lambda)}.
$$

### Vertical subbundle of the fibre bundle
Since we have defined $\forall e\in C^1\times\mathbb{R}:V_e C^1\times\mathbb{R}$, we define the vertical space $VC^1\times\mathbb{R}$ as
$$
VC^1\times\mathbb{R} = \bigcup_{e\in E}\{(e,X)|X\in V_eC^1\times\mathbb{R}\}.
$$
This is a subbundle of $(C^1\times\mathbb{R},\pi,C^1)$. 
#### Chart of the vertical subbundle
We can take the curve and tangent vectors from section [[#Vertical tangent space chart]] and study $VC^1\times \mathbb{R}$ using chart an extended cartesian chart $\tilde{x}:TC^1\times\mathbb{R}\rightarrow \mathbb{R}^6$ where $TC^1\times\mathbb{R}$ is the tangent space of $C^1\times\mathbb{R}$. Then
$$
\tilde{x}(\gamma(\lambda),X_{\gamma,\gamma(\lambda)}) = (r\cos\alpha,r\sin\alpha,z(\lambda),0,0,z'(\lambda)).
$$
This chart is just uses the information we already have i.e. we know $x(\gamma(\lambda))$ and $X_{\gamma,\gamma(\lambda)}$ are in the cartesian chart from section [[#Vertical tangent space chart]]. 

## Horizontal Subbundle (The connection)

### Horizontal tangent space
The choice of a vertical tangent space at a point is fixed by $\pi$. However, the choice of a horizontal tangent space at a point is arbitrary. The only restrictions are
1. $\forall e\in C^1\times\mathbb{R}:V_e C^1\times\mathbb{R}\oplus H_e C^1\times\mathbb{R} = T_e C^1\times\mathbb{R}$.
2. $H_eC^1\times\mathbb{R}$ must vary smoothly w.r.t $e$.

#### Horizontal tangent space chart
Suppose we have a curve $\eta:\mathbb{R}\rightarrow C^1\times\mathbb{R}$ that move along a circle (for example the red circle in the figure). The using the cartesian chart $x$ we have
$$
x(\eta(\lambda)) = (r\cos\theta(\lambda),r\sin\theta(\lambda),b)
$$
where $r$ is a positive real number, $\theta(\lambda)$ is a smooth function that depends $\lambda$ and $b$ is a real number. The tangent vectors of this curve will have form 
$$
X_{\eta,\eta(\lambda)} = -r\theta'(\lambda)\sin\theta(\lambda)(\frac{\partial}{\partial x^1})_{\eta(\lambda)} + r\theta'(\lambda)\cos\theta(\lambda)(\frac{\partial}{\partial x^2})_{\eta(\lambda)}.
$$
For example if $\gamma(0)=\eta(0)=p$ then clearly $V_p C^1\times\mathbb{R}\oplus H_p C^1\times\mathbb{R} = T_p C^1\times\mathbb{R}$. Furthermore these horizontal tangent spaces vary smoothly.

### Horizontal subbundle of the fibrebundle
Now that we chosen horizontal tangent spaces (see section [[#Horizontal tangent space chart]]) we can define the horizontal sub-bundle $H C^1\times\mathbb{R}$ as
$$
H C^1\times\mathbb{R} := \bigcup_{e\in C^1\times\mathbb{R}}\{(e,X)|X\in H_e C^1\times\mathbb{R}\}.
$$
The horizontal subble is known as **Ehresmann conneciton**.

#### Horizontal subbundle chart
We may use the extended cartesian chart defined in section [[#Vertical subbundle of the fibre bundle]]. Then
$$
\tilde{x}(\eta(\lambda),X_{\eta,\eta(\lambda)})=(r\cos\theta(\lambda),r\sin\theta(\lambda),b,-r\theta'(\lambda)\sin\theta(\lambda),r\theta'(\lambda)\cos\theta(\lambda),0)
$$
where the first three coordinates are $x(\eta(\lambda))$ and the last three coordinates are the components of $X_{\eta,\eta(\lambda)}$

