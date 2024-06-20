Suppose $X,Y\in\Gamma(M)$ where $\Gamma(M)$ is the set of vector fields on manifold $M$. We will define the Lie bracket $[X,Y]$ in this note. 

## Definition
*Definiton:* We define $[X,Y]:= X(Y) - Y(X)$. 

### Computing Lie Brackets in coordinates
Suppose we have local chart $(x,U)$ of $M$. Then in coordinates we define 
$$
\begin{aligned}
X(Y) &= X\left(Y^i(x^1,x^2,...,x^n)\frac{\partial}{\partial x^i}\right)\\
&= X^j(x^1,...,x^n)\frac{\partial}{\partial x^j}\left(Y^i(x^1,x^2,...,x^n)\frac{\partial}{\partial x^i}\right)\\
&= X^j(x^1,...,x^n)\frac{\partial }{\partial x^j}Y^i(x^1,...,x^n)\frac{\partial}{\partial x^i}+X^j(x^1,...,x^j)Y^i(x^1,...,x^n)\frac{\partial^2}{\partial x^j\partial x^i}
\end{aligned}
$$
Then we can do the same for 
$$
\begin{aligned}
Y(X) &= Y\left(X^i(x^1,x^2,...,x^n)\frac{\partial}{\partial x^i}\right)\\
&= Y^j(x^1,...,x^n)\frac{\partial}{\partial x^j}\left(X^i(x^1,x^2,...,x^n)\frac{\partial}{\partial x^i}\right)\\
&= Y^j(x^1,...,x^n)\frac{\partial }{\partial x^j}X^i(x^1,...,x^n)\frac{\partial}{\partial x^i}+Y^j(x^1,...,x^j)X^i(x^1,...,x^n)\frac{\partial^2}{\partial x^j\partial x^i}
\end{aligned}
$$
Then 
$$
\begin{aligned}
X(Y)-Y(X)&= X^j(x^1,...,x^n)\frac{\partial }{\partial x^j}Y^i(x^1,...,x^n)\frac{\partial}{\partial x^i}-Y^j(x^1,...,x^n)\frac{\partial }{\partial x^j}X^i(x^1,...,x^n)\frac{\partial}{\partial x^i}\\
&=\left(X^j(x^1,...,x^n)\frac{\partial }{\partial x^j}Y^i(x^1,...,x^n)-Y^j(x^1,...,x^n)\frac{\partial }{\partial x^j}X^i(x^1,...,x^n)\right)\frac{\partial}{\partial x^i}
\end{aligned}
$$
where $X^j,Y^j$ are smooth functions from $\mathbb{R}^{n}\rightarrow \mathbb{R}$. Note that in wikipedia of Lie brackets they say that $X^j,Y^j$ are smooth functions from $M\rightarrow \mathbb{R}$. There seems to be a conflict between our definiton and theirs. This begs the questions can does given a chart $(x,U)$ and $f\in C^\infty(M)$, we can create a function
$$
f\circ x^{-1}(a_1,...,a_n)
$$
where $(a_1,...,a_n)\in\mathbb{R}^n$.  
My idea is the following if $X^j$ is a smooth function from $\mathbb{R}^{n}\rightarrow \mathbb{R}$, could I not create another function that $f^j:M\rightarrow\mathbb{R}$ such that $f^j\circ x^{-1}=X^j$?