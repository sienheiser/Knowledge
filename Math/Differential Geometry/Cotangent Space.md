#DifferentialGeometry
Once we have vector space $T_pM$ we can define the cotangent vector space $T_pM^*$ which is the set  
$$
T_pM^* = \{\phi| \phi:T_pM\tilde{\rightarrow} \mathbb{R} \}
$$

### Example

Let $f \in C^{\infty}(M)$ then 
$$
(df)_p:T_pM \tilde{\rightarrow} \mathbb{R}
$$

So $(df)_p \in T_pM^*$. Now $(df)_p$ is called the gradient of $f$ at $p \in M$.

### Computing components

Suppose we have chart $(U,x)$. Let's take $(df)_p$ and make it eat a vector from $T_pM$.  Then components of the covector are

$$
\begin{aligned}
((df)_p)_j &:= (df)_p(\frac{\partial}{\partial x^j})_p\\
&= (\frac{\partial f}{\partial x^j})_p\\
&= \partial_j(f\circ x^{-1})'(x(p))

\end{aligned}
$$

### Changing charts

Suppose we have covector $\omega$ then 
$$
\begin{aligned}
\omega &= \omega_{(x)i}(dx^i)_p = \omega_{(y)j}(dy^j)_p\\
&\implies \omega_{(y)i} = \frac{\partial x^j}{\partial y^i}\omega_{(x)j}.
\end{aligned}
$$

