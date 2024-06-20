Suppose we have operator $H_0$ and we know its eigenvalues and eigenvectors:
$$
H_0e_{n\delta} = h_ne_{n\delta}
$$
where $n = 1,2,3,....$ (finite or countable) and $\delta = 1,2,...,d(n)$ where $d(n):= \dim \text{Eig}_{H_0}(h_n)$. In simple terms $d(n)$ is the number that tells how many eigenvectors $e_n\delta$ have the same eigenvalues $h_n$. It is important to see that the degenerate eigenvectors form closed subspace that is also a [[Hilbert space]].

To do purtubation of $H_0$ we consider another operator $W$ and $\lambda\in(a,b)$ where $0\in(a,b)$. We want to find eigenvalues and eigenvector of 
$$
H_\lambda := H_0 + \lambda W
$$
where $H_\lambda$ is [[Self-adjoint and adjoint|self-adjoint]] for all possible $\lambda$.

Our end goal is to find
$$
H_\lambda e_{n\delta}(\lambda) = h_{n\delta}(\lambda)e_{n\delta}(\lambda)
$$
where when $\lambda$ is not zero the degenerate eigenvectors become non degenerate.