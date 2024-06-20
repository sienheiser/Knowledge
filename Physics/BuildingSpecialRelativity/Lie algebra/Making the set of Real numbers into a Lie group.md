We use the [[Making a Lie group|recepie]] to make $\mathbb{R}$ into a Lie group. 

## Defining a group action
Since we use the $(\mathbb{R},+)$ group in [[Making a Principal Bundle]], we take it as our example group.

## Defining a topology
The [[The Euclidean Topology on Real numbers|euclidean topology on real numbers]] can be defined on $\mathbb{R}$.

## Making a topological manifold
To make $\mathbb{R}$ into a topological manifold, we will make define charts over $\mathbb{R}$. We may define a global chart on ($\mathbb{R},x)$. Take any $a\in\mathbb{R}$ then define $x(a) = a$. 

## Making a differentiable manifold
If we have multiple charts defined in the previous section, we would then have to check the transistion between charts. Therefore $(\mathbb{R},\mathcal{A})$ with $(\mathbb{R},x)\in\mathcal{A}$ is a differentiable manifold.

## Checking if it is a Lie group

To check if $(\mathbb{R},+)$ is a lie group we need to see if addition map
$$
+:\mathbb{R}\times\mathbb{R}\rightarrow \mathbb{R}
$$
and the inverse map

$$
i:\mathbb{R}\rightarrow \mathbb{R}
$$
where $\forall a\in\mathbb{R}:i(a)=-a$ are smooth maps.

It is clear for this group that both the maps are smooth map

So at this point we have defined a Lie group. We would like to find the Lie algebra of this group.

## Finding Lie algebra

We defined the Lie algebra as a set that contains all the left invariant vector fields of a manifold. We may compute these fields in the following manner.

Take a tangent vector $X_{0}$ at the identity and push the vector forward by an arbitrary amount, that is we want to compute
$$
l_{a*}(X_{0})f
$$
where $l_{a*}$ is the push-forward of the left map, $f\in C^\infty(\mathbb{R})$ is a smooth function. To do any calculations we may employ chart. In this case we have global chart $(x,\mathbb{R})$ defined as $x(b) := b$. Therefore
$$
\begin{aligned}
l_{a*}(X_0)f&\stackrel{1}{=} X_0(f\circ l_a) \\
&\stackrel{2}{=} \left(\frac{\partial}{\partial x^1}\right)_0(f\circ l_a)\\
&\stackrel{3}{=}\partial_1(f\circ l_a\circ x^{-1})(x(0))\\
&\stackrel{4}{=}\partial_1(f\circ x^{-1}\circ x\circ l_a\circ x^{-1})(x(0))\\
&\stackrel{5}{=}\partial_1(x\circ l_a\circ x^{-1})^1(x(0))\partial_1(f\circ x^{-1})(x(a))\\
&\stackrel{6}{=} \partial_1(x\circ l_a\circ x^{-1})^1(x(0))\left(\frac{\partial}{\partial x^1}\right)_a f
\end{aligned}
$$
where $\stackrel{1}{=}$ is true because of the definition of [[Push-forward map]], $\stackrel{2}{=}$ is true because we $X_0$ as tangent vector with component $1$, $\stackrel{3}{=}$ is true because of the definiton of $(\frac{\partial}{\partial x^1}) f$, $\stackrel{4}{=}$ is true because we just inlude the identity map, $\stackrel{5}{=}$ is true because associativity of composition between maps and we took the derivatives and $\stackrel{6}{=}$ is true because of the same reason as $\stackrel{3}{=}$.

Now we need to compute the 
$$
x\circ l_a\circ x^{-1} (x(b))
$$
and take the derivative against the input. So
$$
\begin{aligned}
x\circ l_a\circ x^{-1} (x(b)) &= x\circ l_a(b)\\
&=x\circ(a+b)\\
&=a+b.
\end{aligned}
$$
Therefore
$$
\partial_1(x\circ l_a\circ x^{-1}) (x(b)) = 1 \quad\forall b\in\mathbb{R}.
$$
Therefore we have that
$$
l_{a*}(X_0)f= \left(\frac{\partial}{\partial x^1}\right)_a f.
$$
We have computed out left-invariant field for this Lie group.