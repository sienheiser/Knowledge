#DifferentialGeometry
Let us have a smooth manifold $(M,\mathcal{O},\mathcal{A})$. Given a vector field $X$ on the manifold and function $f\in C^{\infty}(M)$ the directional derivative is given by symbol 
$$
Xf
$$
where this symbol represents us considering all the points simultaneausly. 

We introduce a new notation for the same action
$$
\nabla_{X}f := Xf = df(X)
$$

So now we have three ways to say the same thing and we may see what each notation does 
$$
\begin{aligned}
X:C^{\infty}(M)&\rightarrow C^{\infty}(M)\\
df: \Gamma(TM)&\rightarrow C^{\infty}(M)\\
\nabla_x: C^{\infty}(M)&\rightarrow C^{\infty}(M)\\
\end{aligned}
$$

The first and third equation are the same. The second one is a bit different, it takes a vector field from the set [[gamma(TM)-module]] and then gives a smooth function over the manifold. 

The point is the new notation will help us generalize the concept of a directional derivative to general tensor fields.