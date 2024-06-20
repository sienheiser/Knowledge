
*Definiton:* The exterior derivative $d$ is defined to be the $\mathbb{R}-$linear mapping from $k-$forms to $k+1-$forms that has the following properties
1. $df$ is the differential of $f$ for a $0$-form $f$.
2. $d(df)=0$ for a $0$-form $f$
3. $d(\alpha\wedge\beta)=d\alpha\wedge \beta + (-1)^p\alpha\wedge\beta$ where $\alpha$ is a $p$-form.

*Definiton:* Let $\omega\in\Omega^n(M)$. Then 
$$
d:\Omega^n(M)\rightarrow\Omega^{n+1}(M)
$$
where
$$
\begin{aligned}
d(w)(X_1,...,X_{n+1}) &= \sum_{i=1}^{n+1}(-1)^{i+1}X_i(\omega(X_1,...,\hat{X}_i,...,X_{n+1}))\\
&+\sum_{i<j} \omega([X_i,X_j],X_1,...,\hat{X}_i,...,\hat{X}_j,...,X_{n+1})
\end{aligned}
$$
where $\hat{X}_i$ means that it is removed and 
$$
[X,Y]f=X(Yf)-Y(X(f))
$$
for all $f\in C^\infty(M)$.

## Examples
We have defined a [[Constructing a connection one form|connection one form]] which is a Lie-algebra valued one-form. We will explicity compute $d(w)$ where $w$ is the conneciton one form using charts.

There are two low level structures found in the definition above
$$
[X,Y]f=X(Yf)-Y(X(f))
$$
and
$$
X_i(\omega(X_1,...,\hat{X_i},...,X_{n+1})).
$$
We have not defined what $X(Yf)$ is. Furtermore, we have not defined what $X_i(\omega(X_1,...,\hat{X_i},...,X_{n+1}))$ is.
