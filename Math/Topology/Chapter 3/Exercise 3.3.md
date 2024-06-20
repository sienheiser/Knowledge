![[Exercise331.png]]
a) Suppose that real number $a$ is the infimum of $S$. Then by definition of infimum 
$$
\begin{aligned}
&\forall x\in S:a\leq x\\
\stackrel{1}{\iff}&\forall x\in S:-a\geq -x\\
\stackrel{2}{\iff}&\forall -y\in S:-a\geq y\\
\stackrel{3}{\iff}&\forall y\in T:-a\geq y\\
\end{aligned}
$$
where $\stackrel{1}{\iff}$ is true because we multiply the by -1, $\stackrel{2}{\iff}$ because of redefiniton $y=-x$ and $\stackrel{3}{\iff}$ is true because of definition of $T$. We see that $-a$ is the supremum of the $T$. Since these are all equalites this is true in general. 

b) Suppose $S$ is a subset is a set that is bounded from below. Then by definiton of $T$, $T$ is a set bounded from above. By least upper bound axiom $T$ has a supremum $a$. But by a) we have that $-a$ is infimum of $S$.


![[Exercise333.png]]
*Proof:* Suppose that $(X,\tau)$ is not connected. Then there exists $T\subset X$ that is a clopen set. This means $T\in \tau$ and $X\backslash T\in \tau$. Therefore we have found proper subsets $A,B\subset X: A,B\in\tau: A\cap B = \emptyset\land A\cup B= X$.

Suppose that there exists proper subsets $A,B\subset X: A,B\in\tau : A\cap B=\emptyset\land A\cup B= X$. Then by defintion of [[Math/Topology/Chapter 3/Connected|connected]], $(X,\tau)$ is not connected.


![[Exercise335.png]]
We will show that there no open finite sets. Suppose there exists $A\in\tau$ such that it is finite. Since $\tau$ is a finite closed topology $X\backslash A$ is a closed and finite set. Then we know that $A\cup X\backslash A = X$. But $X$ is an infinite set. This is a contradiction since the union of two finite sets cannot be infinite. Therefore there are no finite open sets. This means that all finite sets are closed. So finite-closed topology is connected.

![[Exercise336.png]]
#ToBeProven 