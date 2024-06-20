*Definiton:*   The exponential of $X\in \mathfrak{g}$ is given by $\exp(X)=\gamma(1)$ where $\gamma:\mathbb{R}\rightarrow G$ is the unique one-parameter subgroup of $G$ whose tangent vector at the identity is equal $X$.

## Example

Let us construct the exponential map for [[Making the set of Real numbers into a Lie group|the set of real numbers with addition as group operation]]. Let $A\in T_0\mathbb{R}$ such that $A = \left(\frac{\partial}{\partial y}_0\right)$. Then we can consturct [[Making the set of Real numbers into a Lie group#Finding Lie algebra|a left invariant vector field]] by 
$$
X^A_b := l_{b*}A.
$$
Where $l_{b*}$ is the [[Push-forward map]] of $l_b(a) = b+a$. 

Let $\gamma^A:\mathbb{R}\rightarrow \mathbb{R}$ be the [[Integral curve|integral curve]] of $X^A$ through point
$$
\gamma^A(0)\stackrel{1}{=}e\stackrel{2}{=}0.
$$
where $\stackrel{1}{=}$ is true because we define it so and $\stackrel{2}{=}$ is true because $0$ is the identity of the set of real numbers with addition as group operation. 

We define the exponential map (of $A$?) to be
$$
\exp(A):=\gamma^A(1).
$$
We know from [[Making the set of Real numbers into a Lie group#Finding Lie algebra|finding Lie algebra]] that 
$$
X^A_b = \left(\frac{\partial}{\partial x}\right)_b.
$$
We need to find an integral curve $\gamma^A$ such that 
$$
X_{\gamma^A,\gamma^A(\lambda)}=\left(\frac{\partial}{\partial x}\right)_\lambda.
$$
Choosing $\gamma^A(\lambda)=\lambda$  satifies the requirements of $\gamma^A(0)=0$ and $X_{\gamma^A,\gamma^A(\lambda)}=\left(\frac{\partial}{\partial x}\right)_\lambda$. Therefore our exponential map is
$$
\exp(tA):=\gamma^A(t)=t
$$

