---
aliases: [homeamorphic intervals]
---

We would like to show that $(a,b)\ncong [a,b]$. To do this we look at the following oberservation. 

Let $f:(X,\tau)\rightarrow (Y,\tau_1)$ be a [[Homeomorphism|homeomorphism]]. Take any $a\in X$ and $b\in Y$. Then $(X\backslash \{a\})\cong(Y\backslash \{b\})$.
*proof:* Define homeomorphism $g: (X\backslash \{a\},\tau_2)\rightarrow (Y\backslash \{f(a)\},\tau_3)$ as $\forall x\in X\backslash \{a\},g(x) = f(x)$ where $\tau_2,\tau_3$ are induced topologies. This $g(x)$ satisfies the properties of [[Homeomorphism|homeomorphism]].

Since $f(x)$ is bijective $g(x)$ is still bijective so (i), (ii) are satisfied. Now we show that for any $U_2\in\tau_2$, $g(U_2)\in \tau_3$. Take any $U_2\in \tau_2$. Then $\exists U\in\tau: U_2= U\cap X\backslash\{a\}$.

Case 1: Suppose that $a\notin U$. Then $U_2 = U\cap X\backslash\{a\} = U$. Then $g(U_2) = f(U_2)=f(U)\in\tau_1$. However since $f(a)\notin f(U)$. Then clearly, $f(U)\cap Y\backslash\{f(a)\}=f(U)$. Therefore $f(U)\in\tau_3$. 

Case 2: Suppose that $a\in U$. Then $U_2 = U\cap X\backslash \{a\}$. Now take $f(U_2)=f(U\cap X\backslash\{a\})$. Then 
$$
\begin{aligned}
f(U\cap X\backslash\{a\}) &\stackrel{1}{=}f(U)\cap f(X\backslash\{a\})\\
&\stackrel{2}{=}f(U)\cap f(X)\backslash(f\{a\})\\
&= f(U)\cap Y\backslash f(\{a\})
\end{aligned}
$$
where we will prove $\stackrel{1}{=},\stackrel{2}{=}$ later. Clearly $f(U)\cap Y\backslash f(\{a\})\in Y\backslash f(\{a\})$. Therefore, $g(x)=f(x),\forall x\in X\backslash \{a\}$ has property (iv) from [[Homeomorphism|homeomorphism]]. The remaning property can be shown in a similar manner. Therefore $(X\backslash\{a\},\tau_2)\cong(Y\backslash f(\{a\},\tau_3))$.

Let $f:X\rightarrow Y$ be a bijection. Then $f(X_1\cap X_2)=f(X_1)\cap f(X_2)$. Take any element $f(x)\in f(X_1\cap X_2)$. This is equivalent to $f^{-1}(f(x))\in X_1\cap X_2$. This is equivalent to $f^{-1}(f(x))\in X_1$ and  $f^{-1}(f(x))\in X_2$. This is equivalent to $f(f^{-1}f(x)))=f(x)\in f(X_1)$ and $f(x)\in f(X_2)$. This is equivalent to $f(x)\in f(X_1)\cap f(x_2)$. We have proven $\stackrel{1}{=}$.

Let $f:X\rightarrow Y$ be a bijection. Then $f(X\backslash \{a\})=f(X)\backslash f(\{a\})$. Take any $f(x)\in f(X\backslash \{a\})$. This is equivalent to $f^{-1}(f(x))=x\in X\backslash\{a\}$. This is equivalent to $x\in X\land x\neq a$. This is equivalent to $f(x)\in f(X)\land f(x)\neq f(a)$. Which is equivalent to $f(x)\in f(X)\backslash f(\{a\})$. We have proven $\stackrel{2}{=}$.


### Intervals which are not homeomorphic
*Corollary:* If $a,b,c,d$ are real numbers such that $a<b$ and $c<d$, then 
1. $(a,b)\ncong [c,d)$,
2. $(a,d)\ncong [c,d]$, and 
3. $[a,b)\ncong [c,d]$.
*proof:*
1. Suppose $f:(a,b)\rightarrow [c,d)$ is [[Homeomorphism|homeomorphism]]. Then by obervation, for some $x\in(a,b)$ and $c\in[c,d)$, $(a,d)\backslash\{x\}\cong[c,d)\backslash\{c\}=(c,d)$. Clearly $(a,d)\backslash\{x\}$ for any $x\in(a,d)$ is not connected. But $(c,d)$ is connected therefore this is a contradiction. Therefore $(a,b)\ncong [c,d)$.
2. Similar to 1.
3. Simirar to 1.


