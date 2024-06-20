#DifferentialGeometry
We have defined the set of all [[Vector Fields|vector fields]] as $\Gamma(TM)$ in [[gamma(TM)]]. Now we equip this set with addition and multiplication to make it a vector space. We may take two vectorfields $\chi, \tilde{\chi}\in\Gamma(TM)$ and define the following operation

$$
\begin{aligned}
(\chi \oplus\tilde{\chi})(f) &= \chi(f)\oplus \tilde{\chi}(f)\\
(g\otimes\chi)(f) &= g\cdot\chi(f)
\end{aligned}
$$
where $f,g\in C^{\infty}(M)$. This is vector space on a ring since $C^{\infty}(M)$ is a ring. A vector space on ring is called a module.  The symbol $X(f)$ means we take the vector field at a point and make it act on the function on the same point for all points. 

The defining feature of a module is that not all modules have a basis.

This is bad because otherwise we could have chosen (for any manifold) vector fields  $\chi_(1),...,\chi_(d)$  write any vector field 
$$
\chi = f^i\chi_{(i)}
$$
where $f^i\in C^{\infty}(M)$. We can find a basis of a vector field locally on the manifold $M$. 

