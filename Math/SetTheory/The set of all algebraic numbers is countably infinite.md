*Theorem:* The set $\mathcal{A}$ of all [[Algebraic and transcedental numbers|algebraic numbers]] is [[Countable, uncountable|countably infinite]].
*Proof:* Let $f(x) = \sum_{i = 0}^{n} a_ix^{n-1}$ where $a_0\neq 0$ and $a_i\in\mathbb{Z}$. Define the height of a polynomial to be $k=n+|a_0|+|a_1|+...+|a_n|$. Now define $A_k$ as the set that contains all the roots of all polynomials that have height $k$. So if some polynomial has height $k$ its roots must belong to $A_k$. Clearly $\mathcal{A} = \cup_{i=1}^\infty A_k$. We show that $A_k$ is finite which results in $\mathcal{A}$ being countably infinite by [[Countable family of countable sets]].

Let $f$ be some polynomial with degree $n$ and height $k$. Clearly, $n\leq k$ and $|a_i|\leq k$ for $i=0,1,2,...,n$. This means there are finitely many polynomials with height $k$. Since a polynomial of degree $n$ has at most $n$ roots then any polynomial with height $k$ can have no more than $k$ roots which is finite. Consequently $A_k$ is finite. Hence $\mathcal{A}$ is countably infinite.


*Corollary:* Every set of algebraic numbers is countably infinite.
Proof: Previous theorem and [[Subset of countable set]].

