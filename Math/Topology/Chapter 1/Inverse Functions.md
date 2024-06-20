---
aliases: [inverse functions, inverse function]
---

*Definiton:* Let $f$ be a funciton that $f:X\mapsto Y$. The function $f$ is said to have an inverse if there exists a function $g$ where $g:Y\mapsto X$ such that $g(f(x)) = x$ for all $x\in X$ and $f(g(y))$ for all $y\in Y$.	The function $g$ is called the **inverse function** of $f$.

*Propositions:* Let us have a map $f:X\mapsto Y$.
1. $f$ is a [[Injective, Surjective and Bijective|bijective]] map if and only if it has an inverse.

*Proof:* We will first start by assuming that $f$ is bijective and show that an $f^{-1}$ function exists. Then we will assume that an inverse function exists and show that $f$ is bijective.

Suppose that $f:X\rightarrow Y$ is bijective. Since $f$ is [[Injective, Surjective and Bijective|surjective]] this means for each $y\in Y$ there exists $x\in X$ such that $f(x) = y$. We define a function $f^{-1}(y) = x$. Since $f:X\rightarrow Y$ is injective, by definiton $f(x_1)=f(x_2)\implies x_1=x_2$. Meaning the $x$ in $f^{-1}(y) = x$ is unique and therefore $f^{-1}:Y\rightarrow X$ is well defined.

We now check if $f^{-1}$ is the inverse function by checking $f^{-1}(f(x)) = x$ and $f(f^{-1}(y)) = y$. Take $x\in X$ then $f(x) = y$ for a unique $y\in Y$. Then by definiton of function $f^{-1}(f(x)) = f^{-1}(y) = x$. Similarly, take a $y\in Y$ then $f^{-1} (y)=x$ for a unique $x\in X$. Then $f(f^{-1}(y)) = f(x)=y$. Therefore we have shown that $f^{-1}$ is the inverse map.

Suppose that $f:X\rightarrow Y$ has an inverse $f^{-1}: Y\rightarrow X$. By definiton we have that $f^{-1}(f(x))=x$, for all $x\in X$ and $f(f^{-1}(y))$ = y, for all $y\in Y$. We show that $f$ is surjective by showing for each $y\in Y$ there exists $x\in X$ such that $f(x) = y$. Take $y\in Y$, by definition of inverse $f^{-1}(y) = x$. This means that $f(x) = f(f^{-1}(y))=y$.

We now show that $f:X\rightarrow Y$ is injective. This means if $f(x_1) = f(x_2)$ then $x_1=x_2$. Take $x_1,x_2\in X$ such that $f(x_1) = f(x_2)$. Then $f(x_1) = y_1$ and $f(x_2) = y_2$ where $y_1,y_2\in Y$. Since $f(x_1) = f(x_2)\implies y_1=y_2=y\in Y$ where $y$ is a relabel. Now $f^{-1}(y_1) = f^{-1}(y)=x_1$ and $f^{-1}(y_2) = f^{-1}(y) = x_2$. Therefore $x_1 = f^{-1}(y)=x_2$.

2. Let us have $g_1:Y\rightarrow X$ and $g_2:Y\rightarrow X$. If $g_1$ and $g_2$ are both inverses of function $f$ show that $g_1=g_2$ for all $y\in Y$.

*Proof:* Since $g_1$ and $g_2$ are inverses of $f$ by definiton of inverse functions $f\circ g_1(y)=y,f\circ g_2(y) = y,g_1\circ f(x)=x$ and $g_2\circ f(x)=x$. Take and $y\in Y$ then  $g_1(y)\in X$. Then $g_1(y) = (g_2\circ f)\circ g_1(y)=g_2\circ(f\circ g_1(y))=g_2(y)$. Therefore we have shown that $g_1=g_2$.

3. Let $g:Y\rightarrow X$. Then $g$ is an inverse of $f:X\rightarrow Y$ if and only if $f$ is an inverse of $g$.

*Proof:* Let $g$ be an inverse of $f$ then by definiton $f(g(y))=y$ for all $y\in Y$ and $g(f(x)) = x$ for all $x\in X$ by definiton. If $f$ is an inverse of $g$ then $f(g(y))=y$ for all $y\in Y$ and $g(f(x))=x$ for all $x\in X$ by definiton. But this is the same as $g$ being inverse of $f$.