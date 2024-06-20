#DifferentialGeometry

An $(r,s)$-tensor field $T$ is a $C^{\infty}(M)$   multilinear map
$$
T:\Gamma(T^*M)\times...\times\Gamma(T^*M)\times\Gamma(TM)\times..\times\Gamma(TM)\tilde{\rightarrow}C^{\infty}(M) 
$$
where $T$ eats $r$ covector field and $s$ vector fields and returns a smooth funtion.

### Example

For $f\in C^{\infty}(M)$ 
$$
\begin{aligned}
df:&\Gamma(TM)\tilde{\rightarrow} C^{\infty}(M)\\
&\chi\rightarrow df(\chi):= \chi f:=(\chi f)(p):= \chi(p)f
\end{aligned}
$$
where $p\in M$ and $\chi(p)\in T_pM$. Note we have a $C^{\infty}(M)$ linear map up there.