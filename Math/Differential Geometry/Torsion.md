Is it possible to use a connection $\nabla$ to define tensors on $(M,\mathcal{O},\mathcal{A},\nabla)$?

*Definition:* The torsion of a connection $\nabla$ is the (1,2)-tensor field
$$
T(\omega,X,Y) := \omega(\nabla_X Y-\nabla_Y X-[X,Y])
$$
where $[X,Y]$ is defined as $[X,Y]f := X(Yf)-Y(Xf)$

Proof that $T$ is $C^{\infty}$ linear in each entry
$$
T(f\omega,X,Y) = f\omega(....) = fT(\omega,X,Y)
$$
For the next arguement
$$
\begin{aligned}
T(\omega,fX,Y) &= \omega(\nabla_{fX}(Y)-\nabla_Y(fX)- [fX,Y])\\
&= \omega(f\nabla_X(Y)-Y(f)X-f\nabla_Y X-[fX,Y])\\
&= \omega(f\nabla_X(Y)-Y(f)X-f\nabla_Y X-f[X,Y]+(Yf)X)\\
&= f\omega(\nabla_X(Y)-\nabla_Y X-[X,Y])\\
&=fT(\omega,X,Y)
\end{aligned}
$$

Similar for other arguments.

